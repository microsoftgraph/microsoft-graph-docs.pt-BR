---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df9298f29e7582a8fa747ba54f74d659de72a65a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060423"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="0cabc-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0cabc-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="0cabc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cabc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cabc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0cabc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cabc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cabc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cabc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0cabc-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0cabc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cabc-108">Properties</span></span>
|<span data-ttu-id="0cabc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cabc-109">Property</span></span>|<span data-ttu-id="0cabc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cabc-110">Type</span></span>|<span data-ttu-id="0cabc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cabc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cabc-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0cabc-112">lastUpdateDateTime</span></span>|<span data-ttu-id="0cabc-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-113">String</span></span>|<span data-ttu-id="0cabc-114">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="0cabc-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="0cabc-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="0cabc-115">contentNamespaceUrl</span></span>|<span data-ttu-id="0cabc-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-116">String</span></span>|<span data-ttu-id="0cabc-117">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="0cabc-117">The DHA report version.</span></span> <span data-ttu-id="0cabc-118">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="0cabc-118">(Namespace version)</span></span>|
|<span data-ttu-id="0cabc-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="0cabc-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="0cabc-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-120">String</span></span>|<span data-ttu-id="0cabc-121">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="0cabc-121">The DHA report version.</span></span> <span data-ttu-id="0cabc-122">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="0cabc-122">(Namespace version)</span></span>|
|<span data-ttu-id="0cabc-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="0cabc-123">contentVersion</span></span>|<span data-ttu-id="0cabc-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-124">String</span></span>|<span data-ttu-id="0cabc-125">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="0cabc-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="0cabc-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cabc-126">issuedDateTime</span></span>|<span data-ttu-id="0cabc-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cabc-127">DateTimeOffset</span></span>|<span data-ttu-id="0cabc-128">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="0cabc-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="0cabc-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="0cabc-129">attestationIdentityKey</span></span>|<span data-ttu-id="0cabc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-130">String</span></span>|<span data-ttu-id="0cabc-131">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="0cabc-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="0cabc-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="0cabc-132">resetCount</span></span>|<span data-ttu-id="0cabc-133">Int64</span><span class="sxs-lookup"><span data-stu-id="0cabc-133">Int64</span></span>|<span data-ttu-id="0cabc-134">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="0cabc-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="0cabc-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="0cabc-135">restartCount</span></span>|<span data-ttu-id="0cabc-136">Int64</span><span class="sxs-lookup"><span data-stu-id="0cabc-136">Int64</span></span>|<span data-ttu-id="0cabc-137">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="0cabc-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="0cabc-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="0cabc-138">dataExcutionPolicy</span></span>|<span data-ttu-id="0cabc-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-139">String</span></span>|<span data-ttu-id="0cabc-140">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="0cabc-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="0cabc-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="0cabc-141">bitLockerStatus</span></span>|<span data-ttu-id="0cabc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-142">String</span></span>|<span data-ttu-id="0cabc-143">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="0cabc-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="0cabc-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="0cabc-144">bootManagerVersion</span></span>|<span data-ttu-id="0cabc-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-145">String</span></span>|<span data-ttu-id="0cabc-146">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="0cabc-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="0cabc-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="0cabc-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="0cabc-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-148">String</span></span>|<span data-ttu-id="0cabc-149">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="0cabc-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="0cabc-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="0cabc-150">secureBoot</span></span>|<span data-ttu-id="0cabc-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-151">String</span></span>|<span data-ttu-id="0cabc-152">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="0cabc-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="0cabc-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="0cabc-153">bootDebugging</span></span>|<span data-ttu-id="0cabc-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-154">String</span></span>|<span data-ttu-id="0cabc-155">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="0cabc-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="0cabc-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="0cabc-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="0cabc-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-157">String</span></span>|<span data-ttu-id="0cabc-158">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="0cabc-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="0cabc-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="0cabc-159">codeIntegrity</span></span>|<span data-ttu-id="0cabc-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-160">String</span></span>| <span data-ttu-id="0cabc-161">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="0cabc-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="0cabc-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="0cabc-162">testSigning</span></span>|<span data-ttu-id="0cabc-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-163">String</span></span>|<span data-ttu-id="0cabc-164">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="0cabc-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="0cabc-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="0cabc-165">safeMode</span></span>|<span data-ttu-id="0cabc-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-166">String</span></span>|<span data-ttu-id="0cabc-167">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="0cabc-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="0cabc-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="0cabc-168">windowsPE</span></span>|<span data-ttu-id="0cabc-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-169">String</span></span>|<span data-ttu-id="0cabc-170">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="0cabc-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="0cabc-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="0cabc-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="0cabc-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-172">String</span></span>|<span data-ttu-id="0cabc-173">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="0cabc-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="0cabc-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="0cabc-174">virtualSecureMode</span></span>|<span data-ttu-id="0cabc-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-175">String</span></span>|<span data-ttu-id="0cabc-176">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="0cabc-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="0cabc-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0cabc-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="0cabc-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-178">String</span></span>|<span data-ttu-id="0cabc-179">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="0cabc-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="0cabc-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="0cabc-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="0cabc-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-181">String</span></span>|<span data-ttu-id="0cabc-182">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="0cabc-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="0cabc-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="0cabc-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="0cabc-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-184">String</span></span>|<span data-ttu-id="0cabc-185">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="0cabc-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="0cabc-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="0cabc-186">tpmVersion</span></span>|<span data-ttu-id="0cabc-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-187">String</span></span>|<span data-ttu-id="0cabc-188">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="0cabc-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="0cabc-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="0cabc-189">pcr0</span></span>|<span data-ttu-id="0cabc-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-190">String</span></span>|<span data-ttu-id="0cabc-191">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="0cabc-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="0cabc-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="0cabc-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="0cabc-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-193">String</span></span>|<span data-ttu-id="0cabc-194">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="0cabc-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="0cabc-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="0cabc-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="0cabc-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-196">String</span></span>|<span data-ttu-id="0cabc-197">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="0cabc-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="0cabc-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="0cabc-198">bootRevisionListInfo</span></span>|<span data-ttu-id="0cabc-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-199">String</span></span>|<span data-ttu-id="0cabc-200">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="0cabc-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="0cabc-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="0cabc-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="0cabc-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-202">String</span></span>|<span data-ttu-id="0cabc-203">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="0cabc-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="0cabc-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="0cabc-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="0cabc-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-205">String</span></span>|<span data-ttu-id="0cabc-206">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="0cabc-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="0cabc-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="0cabc-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="0cabc-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cabc-208">String</span></span>|<span data-ttu-id="0cabc-209">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="0cabc-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cabc-210">Relações</span><span class="sxs-lookup"><span data-stu-id="0cabc-210">Relationships</span></span>
<span data-ttu-id="0cabc-211">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cabc-211">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cabc-212">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cabc-212">JSON Representation</span></span>
<span data-ttu-id="0cabc-213">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cabc-213">Here is a JSON representation of the resource.</span></span>
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






