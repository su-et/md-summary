A simple tool for summarizing SAML federation metadata. It tries to
identify the software running on each IdP and SP using the endpoint
URLs.

### Requirements

* perl 5.20 or newer

### Usage

    md-summary metadata.xml

### Example

    % curl -s -O http://md.incommon.org/InCommon/InCommon-metadata.xml
    % ./md-summary InCommon-metadata.xml
    Identity Providers (1799):
      Shibboleth             1577 ( 87.7%)
      SimpleSAMLphp            88 (  4.9%)
      OpenAthens               77 (  4.3%)
      ADFS                     22 (  1.2%)
      Other                    16 (  0.9%)
      PingFederate              8 (  0.4%)
      Authentic 2               4 (  0.2%)
      IBM Tivoli FIM            3 (  0.2%)
      CA SiteMinder             2 (  0.1%)
      Novell Access Manager     2 (  0.1%)
    Service Providers (5063):
      Shibboleth             4101 ( 81.0%)
      SimpleSAMLphp           372 (  7.3%)
      Other                   199 (  3.9%)
      Philo                    79 (  1.6%)
      OneLogin                 78 (  1.5%)
      Instructure?             72 (  1.4%)
      Atypon Literatum?        35 (  0.7%)
      RSmart OneCampus?        24 (  0.5%)
      ADFS                     24 (  0.5%)
      ExLibris?                12 (  0.2%)
      Kaltura?                 11 (  0.2%)
      iModules?                11 (  0.2%)
      PingFederate             11 (  0.2%)
      UprisingTech?            10 (  0.2%)
      Ingenta?                  7 (  0.1%)
      Cornerstone               7 (  0.1%)
      CA SiteMinder             5 (  0.1%)
      Kuali                     5 (  0.1%)
    %

### Bugs, Issues, etc.

Yes, probably.
