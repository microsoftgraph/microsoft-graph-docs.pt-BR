---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd44dc4e2eb953d09d72f5058139cbf66a08acb9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942091"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="2064d-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="2064d-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="2064d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2064d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2064d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2064d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2064d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2064d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2064d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2064d-107">Properties</span></span>
|<span data-ttu-id="2064d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2064d-108">Property</span></span>|<span data-ttu-id="2064d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2064d-109">Type</span></span>|<span data-ttu-id="2064d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2064d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2064d-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2064d-111">lastUpdateDateTime</span></span>|<span data-ttu-id="2064d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-112">String</span></span>|<span data-ttu-id="2064d-113">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="2064d-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="2064d-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="2064d-114">contentNamespaceUrl</span></span>|<span data-ttu-id="2064d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-115">String</span></span>|<span data-ttu-id="2064d-116">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="2064d-116">The DHA report version.</span></span> <span data-ttu-id="2064d-117">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="2064d-117">(Namespace version)</span></span>|
|<span data-ttu-id="2064d-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="2064d-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="2064d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-119">String</span></span>|<span data-ttu-id="2064d-120">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="2064d-120">The DHA report version.</span></span> <span data-ttu-id="2064d-121">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="2064d-121">(Namespace version)</span></span>|
|<span data-ttu-id="2064d-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="2064d-122">contentVersion</span></span>|<span data-ttu-id="2064d-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-123">String</span></span>|<span data-ttu-id="2064d-124">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="2064d-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="2064d-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="2064d-125">issuedDateTime</span></span>|<span data-ttu-id="2064d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2064d-126">DateTimeOffset</span></span>|<span data-ttu-id="2064d-127">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="2064d-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="2064d-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="2064d-128">attestationIdentityKey</span></span>|<span data-ttu-id="2064d-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-129">String</span></span>|<span data-ttu-id="2064d-130">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="2064d-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="2064d-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="2064d-131">resetCount</span></span>|<span data-ttu-id="2064d-132">Int64</span><span class="sxs-lookup"><span data-stu-id="2064d-132">Int64</span></span>|<span data-ttu-id="2064d-133">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="2064d-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="2064d-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="2064d-134">restartCount</span></span>|<span data-ttu-id="2064d-135">Int64</span><span class="sxs-lookup"><span data-stu-id="2064d-135">Int64</span></span>|<span data-ttu-id="2064d-136">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="2064d-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="2064d-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="2064d-137">dataExcutionPolicy</span></span>|<span data-ttu-id="2064d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-138">String</span></span>|<span data-ttu-id="2064d-139">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="2064d-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="2064d-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="2064d-140">bitLockerStatus</span></span>|<span data-ttu-id="2064d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-141">String</span></span>|<span data-ttu-id="2064d-142">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="2064d-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="2064d-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="2064d-143">bootManagerVersion</span></span>|<span data-ttu-id="2064d-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-144">String</span></span>|<span data-ttu-id="2064d-145">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="2064d-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="2064d-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="2064d-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="2064d-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-147">String</span></span>|<span data-ttu-id="2064d-148">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="2064d-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="2064d-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="2064d-149">secureBoot</span></span>|<span data-ttu-id="2064d-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-150">String</span></span>|<span data-ttu-id="2064d-151">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="2064d-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="2064d-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="2064d-152">bootDebugging</span></span>|<span data-ttu-id="2064d-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-153">String</span></span>|<span data-ttu-id="2064d-154">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="2064d-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="2064d-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="2064d-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="2064d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-156">String</span></span>|<span data-ttu-id="2064d-157">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="2064d-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="2064d-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="2064d-158">codeIntegrity</span></span>|<span data-ttu-id="2064d-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-159">String</span></span>| <span data-ttu-id="2064d-160">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="2064d-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="2064d-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="2064d-161">testSigning</span></span>|<span data-ttu-id="2064d-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-162">String</span></span>|<span data-ttu-id="2064d-163">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="2064d-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="2064d-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="2064d-164">safeMode</span></span>|<span data-ttu-id="2064d-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-165">String</span></span>|<span data-ttu-id="2064d-166">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="2064d-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="2064d-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="2064d-167">windowsPE</span></span>|<span data-ttu-id="2064d-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-168">String</span></span>|<span data-ttu-id="2064d-169">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="2064d-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="2064d-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="2064d-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="2064d-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-171">String</span></span>|<span data-ttu-id="2064d-172">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="2064d-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="2064d-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="2064d-173">virtualSecureMode</span></span>|<span data-ttu-id="2064d-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-174">String</span></span>|<span data-ttu-id="2064d-175">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="2064d-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="2064d-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2064d-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="2064d-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-177">String</span></span>|<span data-ttu-id="2064d-178">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="2064d-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="2064d-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="2064d-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="2064d-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-180">String</span></span>|<span data-ttu-id="2064d-181">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="2064d-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="2064d-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="2064d-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="2064d-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-183">String</span></span>|<span data-ttu-id="2064d-184">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="2064d-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="2064d-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="2064d-185">tpmVersion</span></span>|<span data-ttu-id="2064d-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-186">String</span></span>|<span data-ttu-id="2064d-187">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="2064d-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="2064d-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="2064d-188">pcr0</span></span>|<span data-ttu-id="2064d-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-189">String</span></span>|<span data-ttu-id="2064d-190">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="2064d-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="2064d-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="2064d-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="2064d-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-192">String</span></span>|<span data-ttu-id="2064d-193">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="2064d-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="2064d-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="2064d-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="2064d-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-195">String</span></span>|<span data-ttu-id="2064d-196">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="2064d-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="2064d-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="2064d-197">bootRevisionListInfo</span></span>|<span data-ttu-id="2064d-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-198">String</span></span>|<span data-ttu-id="2064d-199">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="2064d-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="2064d-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="2064d-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="2064d-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-201">String</span></span>|<span data-ttu-id="2064d-202">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="2064d-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="2064d-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="2064d-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="2064d-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-204">String</span></span>|<span data-ttu-id="2064d-205">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="2064d-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="2064d-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="2064d-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="2064d-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2064d-207">String</span></span>|<span data-ttu-id="2064d-208">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="2064d-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="2064d-209">Relações</span><span class="sxs-lookup"><span data-stu-id="2064d-209">Relationships</span></span>
<span data-ttu-id="2064d-210">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2064d-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2064d-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2064d-211">JSON Representation</span></span>
<span data-ttu-id="2064d-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2064d-212">Here is a JSON representation of the resource.</span></span>
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




