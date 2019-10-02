---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26070efb2247ef1fdfa60f45a985eb9223de923b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356958"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="7a4f4-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="7a4f4-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="7a4f4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a4f4-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a4f4-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7a4f4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a4f4-106">Properties</span></span>
|<span data-ttu-id="7a4f4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a4f4-107">Property</span></span>|<span data-ttu-id="7a4f4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a4f4-108">Type</span></span>|<span data-ttu-id="7a4f4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a4f4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a4f4-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4f4-110">lastUpdateDateTime</span></span>|<span data-ttu-id="7a4f4-111">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-111">String</span></span>|<span data-ttu-id="7a4f4-112">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="7a4f4-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="7a4f4-113">contentNamespaceUrl</span></span>|<span data-ttu-id="7a4f4-114">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-114">String</span></span>|<span data-ttu-id="7a4f4-115">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-115">The DHA report version.</span></span> <span data-ttu-id="7a4f4-116">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="7a4f4-116">(Namespace version)</span></span>|
|<span data-ttu-id="7a4f4-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="7a4f4-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="7a4f4-118">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-118">String</span></span>|<span data-ttu-id="7a4f4-119">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-119">The DHA report version.</span></span> <span data-ttu-id="7a4f4-120">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="7a4f4-120">(Namespace version)</span></span>|
|<span data-ttu-id="7a4f4-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="7a4f4-121">contentVersion</span></span>|<span data-ttu-id="7a4f4-122">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-122">String</span></span>|<span data-ttu-id="7a4f4-123">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="7a4f4-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="7a4f4-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a4f4-124">issuedDateTime</span></span>|<span data-ttu-id="7a4f4-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a4f4-125">DateTimeOffset</span></span>|<span data-ttu-id="7a4f4-126">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="7a4f4-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="7a4f4-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="7a4f4-127">attestationIdentityKey</span></span>|<span data-ttu-id="7a4f4-128">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-128">String</span></span>|<span data-ttu-id="7a4f4-129">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="7a4f4-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="7a4f4-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="7a4f4-130">resetCount</span></span>|<span data-ttu-id="7a4f4-131">Int64</span><span class="sxs-lookup"><span data-stu-id="7a4f4-131">Int64</span></span>|<span data-ttu-id="7a4f4-132">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="7a4f4-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="7a4f4-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="7a4f4-133">restartCount</span></span>|<span data-ttu-id="7a4f4-134">Int64</span><span class="sxs-lookup"><span data-stu-id="7a4f4-134">Int64</span></span>|<span data-ttu-id="7a4f4-135">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="7a4f4-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="7a4f4-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="7a4f4-136">dataExcutionPolicy</span></span>|<span data-ttu-id="7a4f4-137">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-137">String</span></span>|<span data-ttu-id="7a4f4-138">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="7a4f4-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="7a4f4-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="7a4f4-139">bitLockerStatus</span></span>|<span data-ttu-id="7a4f4-140">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-140">String</span></span>|<span data-ttu-id="7a4f4-141">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="7a4f4-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="7a4f4-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="7a4f4-142">bootManagerVersion</span></span>|<span data-ttu-id="7a4f4-143">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-143">String</span></span>|<span data-ttu-id="7a4f4-144">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="7a4f4-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="7a4f4-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="7a4f4-146">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-146">String</span></span>|<span data-ttu-id="7a4f4-147">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="7a4f4-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="7a4f4-148">secureBoot</span></span>|<span data-ttu-id="7a4f4-149">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-149">String</span></span>|<span data-ttu-id="7a4f4-150">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="7a4f4-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="7a4f4-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="7a4f4-151">bootDebugging</span></span>|<span data-ttu-id="7a4f4-152">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-152">String</span></span>|<span data-ttu-id="7a4f4-153">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="7a4f4-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="7a4f4-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="7a4f4-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="7a4f4-155">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-155">String</span></span>|<span data-ttu-id="7a4f4-156">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="7a4f4-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="7a4f4-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="7a4f4-157">codeIntegrity</span></span>|<span data-ttu-id="7a4f4-158">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-158">String</span></span>| <span data-ttu-id="7a4f4-159">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="7a4f4-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="7a4f4-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="7a4f4-160">testSigning</span></span>|<span data-ttu-id="7a4f4-161">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-161">String</span></span>|<span data-ttu-id="7a4f4-162">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="7a4f4-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="7a4f4-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="7a4f4-163">safeMode</span></span>|<span data-ttu-id="7a4f4-164">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-164">String</span></span>|<span data-ttu-id="7a4f4-165">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="7a4f4-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="7a4f4-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="7a4f4-166">windowsPE</span></span>|<span data-ttu-id="7a4f4-167">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-167">String</span></span>|<span data-ttu-id="7a4f4-168">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="7a4f4-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="7a4f4-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="7a4f4-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="7a4f4-170">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-170">String</span></span>|<span data-ttu-id="7a4f4-171">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="7a4f4-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="7a4f4-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="7a4f4-172">virtualSecureMode</span></span>|<span data-ttu-id="7a4f4-173">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-173">String</span></span>|<span data-ttu-id="7a4f4-174">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="7a4f4-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="7a4f4-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7a4f4-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="7a4f4-176">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-176">String</span></span>|<span data-ttu-id="7a4f4-177">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="7a4f4-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="7a4f4-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="7a4f4-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="7a4f4-179">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-179">String</span></span>|<span data-ttu-id="7a4f4-180">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="7a4f4-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="7a4f4-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="7a4f4-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="7a4f4-182">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-182">String</span></span>|<span data-ttu-id="7a4f4-183">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="7a4f4-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="7a4f4-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="7a4f4-184">tpmVersion</span></span>|<span data-ttu-id="7a4f4-185">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-185">String</span></span>|<span data-ttu-id="7a4f4-186">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="7a4f4-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="7a4f4-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="7a4f4-187">pcr0</span></span>|<span data-ttu-id="7a4f4-188">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-188">String</span></span>|<span data-ttu-id="7a4f4-189">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="7a4f4-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="7a4f4-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="7a4f4-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="7a4f4-191">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-191">String</span></span>|<span data-ttu-id="7a4f4-192">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="7a4f4-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="7a4f4-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="7a4f4-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="7a4f4-194">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-194">String</span></span>|<span data-ttu-id="7a4f4-195">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="7a4f4-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="7a4f4-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="7a4f4-196">bootRevisionListInfo</span></span>|<span data-ttu-id="7a4f4-197">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-197">String</span></span>|<span data-ttu-id="7a4f4-198">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="7a4f4-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="7a4f4-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="7a4f4-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="7a4f4-200">String</span><span class="sxs-lookup"><span data-stu-id="7a4f4-200">String</span></span>|<span data-ttu-id="7a4f4-201">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="7a4f4-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="7a4f4-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="7a4f4-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="7a4f4-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a4f4-203">String</span></span>|<span data-ttu-id="7a4f4-204">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="7a4f4-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="7a4f4-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="7a4f4-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="7a4f4-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a4f4-206">String</span></span>|<span data-ttu-id="7a4f4-207">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="7a4f4-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a4f4-208">Relações</span><span class="sxs-lookup"><span data-stu-id="7a4f4-208">Relationships</span></span>
<span data-ttu-id="7a4f4-209">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a4f4-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a4f4-210">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a4f4-210">JSON Representation</span></span>
<span data-ttu-id="7a4f4-211">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a4f4-211">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```




