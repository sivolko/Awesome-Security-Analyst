# STRIDE

S : Spoofing

T : Tampering

R : Repudiation

I : Information Disclosure

D : Denial of Service (DOS)

E : Elevation of Privilege

**Developed by Loren Kohnfelder and Praerit Garg in 1999** to identidy potential vulnerabilities and threats to your products

|       | **Type of Threat**      | **Violation**    | **How**                                                                |
| ----- | ----------------------- | ---------------- | ---------------------------------------------------------------------- |
| **S** | Spoofing                | Authentication   | Impersonating something or someone knwon and trusted                   |
| **T** | Tampering               | Integrity        | Modifying data on disk, Memory, Netowrk etc                            |
| **R** | Repudiation             | Non- repudiation | Claims to not be responsible for an action                             |
| **I** | Information Disclosure  | Confidentiality  | Providing information to someone who is not authorised                 |
| **D** | Denial of Service (DoS) | Availability     | Denying or obstructing access to resources required to provide service |
| **E** | Elevation of Privilege  | Authorization    | Allowing access to someone without proper authorization                |

Tips for identifying Threats&#x20;

<details>

<summary>Start with External Entities </summary>

* Identify and prioritize external entities or events that drive activity.
* Use external drivers as a starting point for threat analysis.

</details>

<details>

<summary>Organisation </summary>

* Organize the threat analysis to ensure completeness.
* Consider going through the diagram in STRIDE order (Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege).
* Avoid over-structuring to maintain creativity.

</details>

<details>

<summary><strong>Record All Threats</strong></summary>

* Write down threats as they arise, even if they are not the primary focus at the moment.
* Revisit recorded threats later to ensure nothing is missed.
* Redundancy helps to avoid overlooking important threats.
* Categorize threats, but don't stress too much about perfect classification (e.g., spoofing vs. information disclosure).

</details>

<details>

<summary>Focus on Feasible Threats </summary>



* Prioritize threats that are more likely to occur and can be addressed.
* Consider the feasibility of mitigating unlikely but possible threats.
* Real-world exploit scenarios should take precedence over less likely but theoretically possible threats.

</details>

## <mark style="color:blue;">4 Types of Actions against each Threats</mark>&#x20;

1. Mitigate it
2. Eliminate it
3. Transfer it&#x20;
4. Accept it&#x20;

### Mitigating VS Eliminating Threats in Threat Modeling

When it comes to securing systems, the approach to dealing with threats involves both mitigating and eliminating them. Here's a brief, technical overview of these strategies:

* **Mitigating Threats**:
  * **Purpose**: Make it harder to exploit a threat.
  * **Example**:
    * Requiring passwords to control login access mitigates the threat of spoofing.
    * Implementing password controls (e.g., complexity requirements, expiration policies) reduces the likelihood of password guessing or misuse if stolen.
* **Eliminating Threats**:
  * **Purpose**: Completely remove the threat.
  * **Example**:
    * **Administrative Access via URL**:
      * **Mitigation**: Use passwords or other authentication methods.
      * **Obfuscation**: Change URL to a non-obvious string (e.g., `/j8e8vg21euwq/`).
      * **Elimination**: Remove the web interface; handle administration via command line.
    * **Moving Away from HTTP**:
      * Reduces the attack surface, making threats easier to mitigate.
* **Key Considerations**:
  * **Threat Analysis**: Identify which threats can be mitigated and which need to be eliminated.
  * **Feasibility**: Consider the likelihood and practicality of addressing each threat.
  * **Comprehensive Models**: Ensure a complete threat model to account for various scenarios, even if certain threats are unlikely.
