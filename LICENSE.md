EARLIFY HEALTH SOURCE AVAILABLE LICENSE
Version 1.0, March 2026

Copyright (c) 2026 Earlify Health S.L.
Dr. Frank Alberto Betances Reinoso — Founder & CSO
Hospital Ribera Polusa, Lugo, Spain

================================================================================

DEFINITIONS

"Software" means the source code, documentation, configuration files, clinical
protocols, machine learning model architectures, and all other materials made
available in this repository.

"Licensor" means Earlify Health S.L. and its authorized representatives.

"You" means the individual or legal entity exercising the rights granted by
this License.

"Commercial Use" means any use of the Software, in whole or in part, intended
for or directed toward commercial advantage or monetary compensation, including
but not limited to: incorporating the Software into a commercial product or
service, offering the Software as a hosted or managed service, using the
Software to provide services to third parties for a fee, or using the Software
in a for-profit organization's internal operations.

"Clinical Deployment" means any use of the Software, or a derivative thereof,
in a real or simulated clinical, therapeutic, or screening context involving
human subjects, patients, or healthcare professionals, regardless of whether
such use is commercial or non-commercial.

"Certified Version" means a version of the Software that has obtained the
applicable regulatory approvals required by the jurisdiction of deployment
(including, but not limited to, CE Marking under EU MDR 2017/745 for
deployment within the European Economic Area).

================================================================================

GRANT OF RIGHTS

Subject to the terms and conditions of this License, the Licensor hereby
grants You a worldwide, royalty-free, non-exclusive, non-transferable license
to:

  1. Access and read the Software for the purposes of evaluation, research,
     academic study, and personal learning.

  2. Fork and modify the Software for non-commercial research or educational
     purposes, provided that all modifications remain subject to this License
     and are clearly marked as modified from the original.

  3. Contribute modifications back to the Licensor's official repository,
     subject to the Contributor Agreement described below.

================================================================================

RESTRICTIONS

You may NOT, without prior written permission from the Licensor:

  1. COMMERCIAL USE
     Use the Software or any derivative work for Commercial Use of any kind.
     This includes, without limitation, offering it as a SaaS platform,
     integrating it into a commercial product, or providing consulting or
     professional services based substantially on the Software.

  2. CLINICAL DEPLOYMENT WITHOUT CERTIFICATION
     Deploy, operate, or make available any Clinical Deployment of the Software
     or any derivative work unless:
       (a) that version is a Certified Version with the applicable regulatory
           approval for the target jurisdiction; AND
       (b) You have obtained prior written authorization from the Licensor.

     This restriction exists to protect patient safety. Deploying uncertified
     clinical decision support software on pediatric populations may cause
     direct harm and constitutes a violation of EU MDR 2017/745 and equivalent
     regulations. This clause applies regardless of whether the deployment is
     commercial or non-commercial.

  3. REDISTRIBUTION AS COMPETING PRODUCT
     Distribute, sublicense, or make available the Software or substantial
     portions thereof as a standalone product or as part of a product that
     competes, directly or indirectly, with the Licensor's products (VIA+,
     VALERIA+, MAGIC, or successor products).

  4. REMOVAL OF NOTICES
     Remove, alter, or obscure any copyright notice, license notice, trademark,
     or attribution notice contained in the Software.

  5. TRADEMARK USE
     Use the names "Earlify Health", "VIA+", "VALERIA+", or "MAGIC" to
     endorse or promote products or services derived from this Software without
     prior written permission from the Licensor.

================================================================================

CLINICAL AND SCIENTIFIC ATTRIBUTION

If You use the Software, its architecture, algorithms, clinical protocols, or
methodology as the basis for a scientific publication, clinical study, thesis,
conference presentation, or equivalent academic output, You must include the
following attribution:

  Betances Reinoso, F.A. et al. (2026). Earlify Health: A Pediatric Digital
  Health Ecosystem for Early Detection and Adaptive Rehabilitation of
  Neurodevelopmental Conditions. Earlify Health S.L., Lugo, Spain.
  https://github.com/earlify-health

================================================================================

CONTRIBUTOR AGREEMENT

By submitting a pull request, patch, or any other contribution to this
repository, You agree that:

  1. Your contribution is Your original work and You have the right to license
     it under the terms of this License.

  2. You grant the Licensor a perpetual, worldwide, royalty-free, irrevocable
     license to use, reproduce, modify, distribute, and sublicense Your
     contribution as part of the Software, including in commercial versions.

  3. You understand that contributing to this repository does not grant You
     any rights beyond those explicitly stated in this License.

  4. You acknowledge that any contribution touching the clinical decision
     logic, machine learning models, or clinical protocols of the Software
     must be reviewed and approved by the Licensor's Chief Scientific Officer
     before being merged, as required by the Software's regulatory obligations
     under EU MDR 2017/745 and EU AI Act 2024/1689.

================================================================================

DISCLAIMER OF WARRANTIES

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.

THE LICENSOR EXPRESSLY DISCLAIMS ANY WARRANTY THAT THE SOFTWARE IS SUITABLE
FOR CLINICAL USE. THE SOFTWARE, IN ITS CURRENT FORM (TRL 5), HAS NOT OBTAINED
CE MARKING UNDER EU MDR 2017/745. IT MUST NOT BE USED FOR CLINICAL DECISION-
MAKING, DIAGNOSIS, OR PATIENT MANAGEMENT WITHOUT REGULATORY AUTHORIZATION.

================================================================================

LIMITATION OF LIABILITY

IN NO EVENT SHALL THE LICENSOR BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES ARISING OUT OF OR IN CONNECTION
WITH THE USE OR INABILITY TO USE THE SOFTWARE, EVEN IF THE LICENSOR HAS BEEN
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

================================================================================

GOVERNING LAW AND JURISDICTION

This License shall be governed by and construed in accordance with the laws of
the Kingdom of Spain, without regard to its conflict of law provisions. Any
dispute arising under this License shall be subject to the exclusive
jurisdiction of the courts of Lugo, Spain.

================================================================================

COMMERCIAL LICENSING AND PARTNERSHIPS

To obtain a commercial license, to discuss research collaborations, or to
inquire about certified clinical deployments, please contact:

  Earlify Health S.L.
  Attn: Dr. Frank Alberto Betances Reinoso, Founder & CSO
  Hospital Ribera Polusa, Lugo, Spain
  fbetances@futureforkids.eu
  https://futureforkids.eu

  ================================================================================
EARLIFY HEALTH — THIRD-PARTY NOTICES
================================================================================

Earlify Health incorporates components from the following open-source projects.
Each component is subject to its own license terms as indicated below.

--------------------------------------------------------------------------------
OpenAI Whisper
Copyright (c) 2022 OpenAI
License: MIT License
https://github.com/openai/whisper
Used in: VALERIA+ — Motor de Reconocimiento de Voz (ASR)
--------------------------------------------------------------------------------
Parselmouth
Copyright (c) 2018–2024 Yannick Jadoul
License: GNU General Public License v3.0
https://github.com/YannickJadoul/Parselmouth
Used in: VIA+ — Motor de Análisis Acústico
Note: Parselmouth is a Python wrapper for Praat (Paul Boersma & David Weenink,
      https://www.praat.org). Praat is distributed under GPLv2+.
--------------------------------------------------------------------------------
openSMILE
Copyright (c) 2008–2023 audEERING GmbH
License: See https://audeering.github.io/opensmile/get-started.html
https://github.com/audeering/opensmile
Used in: VIA+ — Motor de Análisis Acústico
Note: Academic/research use. Commercial use requires a separate license from
      audEERING GmbH. Earlify Health operates under a commercial license
      agreement with audEERING for production use.
--------------------------------------------------------------------------------
librosa
Copyright (c) 2013–2024 librosa development team
License: ISC License
https://github.com/librosa/librosa
Used in: VIA+ — Generador de Espectrogramas
--------------------------------------------------------------------------------
scikit-learn
Copyright (c) 2007–2024 The scikit-learn developers
License: BSD 3-Clause License
https://scikit-learn.org
Used in: VIA+ — Clasificador ML por Dominio Funcional
--------------------------------------------------------------------------------
XGBoost
Copyright (c) 2014–2024 XGBoost contributors
License: Apache License 2.0
https://github.com/dmlc/xgboost
Used in: VIA+ — Clasificador ML por Dominio Funcional
--------------------------------------------------------------------------------
SHAP (SHapley Additive exPlanations)
Copyright (c) 2018 Scott Lundberg
License: MIT License
https://github.com/shap/shap
Used in: VIA+ — Explicabilidad del CDSS (AI Act compliance)
--------------------------------------------------------------------------------
Unity Engine
Copyright (c) 2024 Unity Technologies
License: Unity Terms of Service (commercial license)
https://unity.com
Used in: MAGIC — Motor de Realidad Aumentada
--------------------------------------------------------------------------------
AR Foundation (Unity)
Copyright (c) 2024 Unity Technologies
License: Unity Package Distribution License
https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@latest
Used in: MAGIC — Motor de Realidad Aumentada (ARKit/ARCore layer)
--------------------------------------------------------------------------------
React Native
Copyright (c) Meta Platforms, Inc. and affiliates
License: MIT License
https://reactnative.dev
Used in: VIA+ · VALERIA+ — Aplicaciones móviles multiplataforma
--------------------------------------------------------------------------------
Node.js
Copyright (c) Node.js contributors
License: MIT License
https://nodejs.org
Used in: Backend unificado
--------------------------------------------------------------------------------
MLflow
Copyright (c) Databricks, Inc.
License: Apache License 2.0
https://mlflow.org
Used in: VIA+ — Trazabilidad de modelos ML (MDR + AI Act compliance)
--------------------------------------------------------------------------------

================================================================================
REGULATORY NOTICE
================================================================================

This software is being developed as a Software as a Medical Device (SaMD)
under EU MDR 2017/745. It is currently at Technology Readiness Level (TRL) 5
and HAS NOT YET obtained CE Marking.

This software MUST NOT be used for clinical decision-making, patient screening,
or any healthcare application involving human subjects until the applicable
regulatory approvals have been obtained and communicated by Earlify Health S.L.

For the current regulatory status of each module (VIA+, VALERIA+, MAGIC),
refer to: https://github.com/earlify-health/wiki/Estrategia-Regulatoria

================================================================================
End of NOTICE
================================================================================


================================================================================

End of Earlify Health Source Available License, Version 1.0
