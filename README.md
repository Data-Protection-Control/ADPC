<img src="assets/adpc_logo_high.png" alt="ADPC" width="50%">

# ADPC

Advanced Data Protection Control (ADPC) is an open specification for the automated, machine-readable communication of users’ privacy decisions and data controllers’ responses. It provides a standard communication layer between services and the user-side software that represents the person, such as a browser, browser extension, operating-system component, personal privacy assistant, or comparable user agent.

ADPC addresses privacy interactions that are currently handled through repetitive website-controlled interfaces, especially cookie banners. Instead of requiring users to answer similar requests manually across websites, ADPC allows services to publish the purposes for which they request a decision and allows user-side software to communicate the user’s choices in a structured, auditable, and interoperable way.

The ADPC specification defines a method for expressing decisions about personal data processing under the European Union’s General Data Protection Regulation (GDPR), the ePrivacy Directive, and comparable privacy frameworks outside the EU. It supports consent, refusal or decline of consent requests, withdrawal of previously given consent, and objection to processing where a right to object applies, including direct marketing based on legitimate interests.

ADPC is purpose-specific and controller-specific. It is not a single global opt-out flag. Controllers can describe their own purposes or use standardised purpose vocabularies, while users remain able to make granular choices for particular services, domains, purposes, and request identifiers.

The core web mechanism currently uses HTTP headers between the user agent and the web server, with an equivalent JavaScript interface for web applications. ADPC-Core does not itself decide the legal effect of a signal and does not replace the substantive requirements of data-protection law. Legal-effect profiles can map ADPC actions to a particular regulatory environment and define how signals should be interpreted under that framework.

ADPC was developed against GDPR and ePrivacy problems, and the European Commission’s proposed GDPR Article 88b makes the need for automated and machine-readable communication of data-subject choices more explicit. The proposal reinforces the role of open technical specifications for rights such as consent, refusal, withdrawal, and objection, while ADPC itself remains a general technical mechanism that is not limited to EU law.

ADPC aims to reduce friction for users and implementation costs for organisations. Users can manage privacy decisions through software they control or trust, while publishers and service providers can receive structured signals that connect to existing consent-management, content-management, and compliance workflows. ADPC does not by itself guarantee legal compliance: controllers remain responsible for providing the required information, establishing the applicable legal basis, respecting user choices, and meeting all other legal obligations.

## Implementations and related projects

- ADPC WordPress Plugin: https://github.com/Data-Protection-Control/ADPC-Wordpress — a WordPress implementation that publishes consent requests, exposes the ADPC discovery header, logs incoming ADPC headers, and bridges ADPC signals to existing consent-management workflows.
- ADPC website: https://www.dataprotectioncontrol.org — background, explanation, and links to specification resources and sample implementations.
- Other implementations can be found: https://github.com/Data-Protection-Control
- Additional implementations for IoT, mixed reality, children’s services, and AI systems will be added to this list soon.

## More information

You can find more information about ADPC on the project website: https://www.dataprotectioncontrol.org
