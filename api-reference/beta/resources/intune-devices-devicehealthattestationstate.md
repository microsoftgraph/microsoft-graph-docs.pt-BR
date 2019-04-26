---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66a22d0d3cc5caa53c41607da1d1de8185f22a62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570086"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="65253-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="65253-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="65253-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65253-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65253-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="65253-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="65253-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65253-107">Properties</span></span>
|<span data-ttu-id="65253-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65253-108">Property</span></span>|<span data-ttu-id="65253-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="65253-109">Type</span></span>|<span data-ttu-id="65253-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65253-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65253-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="65253-111">lastUpdateDateTime</span></span>|<span data-ttu-id="65253-112">String</span><span class="sxs-lookup"><span data-stu-id="65253-112">String</span></span>|<span data-ttu-id="65253-113">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="65253-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="65253-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="65253-114">contentNamespaceUrl</span></span>|<span data-ttu-id="65253-115">String</span><span class="sxs-lookup"><span data-stu-id="65253-115">String</span></span>|<span data-ttu-id="65253-116">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="65253-116">The DHA report version.</span></span> <span data-ttu-id="65253-117">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="65253-117">(Namespace version)</span></span>|
|<span data-ttu-id="65253-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="65253-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="65253-119">String</span><span class="sxs-lookup"><span data-stu-id="65253-119">String</span></span>|<span data-ttu-id="65253-120">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="65253-120">The DHA report version.</span></span> <span data-ttu-id="65253-121">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="65253-121">(Namespace version)</span></span>|
|<span data-ttu-id="65253-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="65253-122">contentVersion</span></span>|<span data-ttu-id="65253-123">String</span><span class="sxs-lookup"><span data-stu-id="65253-123">String</span></span>|<span data-ttu-id="65253-124">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="65253-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="65253-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="65253-125">issuedDateTime</span></span>|<span data-ttu-id="65253-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65253-126">DateTimeOffset</span></span>|<span data-ttu-id="65253-127">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="65253-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="65253-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="65253-128">attestationIdentityKey</span></span>|<span data-ttu-id="65253-129">String</span><span class="sxs-lookup"><span data-stu-id="65253-129">String</span></span>|<span data-ttu-id="65253-130">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="65253-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="65253-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="65253-131">resetCount</span></span>|<span data-ttu-id="65253-132">Int64</span><span class="sxs-lookup"><span data-stu-id="65253-132">Int64</span></span>|<span data-ttu-id="65253-133">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="65253-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="65253-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="65253-134">restartCount</span></span>|<span data-ttu-id="65253-135">Int64</span><span class="sxs-lookup"><span data-stu-id="65253-135">Int64</span></span>|<span data-ttu-id="65253-136">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="65253-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="65253-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="65253-137">dataExcutionPolicy</span></span>|<span data-ttu-id="65253-138">String</span><span class="sxs-lookup"><span data-stu-id="65253-138">String</span></span>|<span data-ttu-id="65253-139">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="65253-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="65253-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="65253-140">bitLockerStatus</span></span>|<span data-ttu-id="65253-141">String</span><span class="sxs-lookup"><span data-stu-id="65253-141">String</span></span>|<span data-ttu-id="65253-142">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="65253-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="65253-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="65253-143">bootManagerVersion</span></span>|<span data-ttu-id="65253-144">String</span><span class="sxs-lookup"><span data-stu-id="65253-144">String</span></span>|<span data-ttu-id="65253-145">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="65253-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="65253-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="65253-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="65253-147">String</span><span class="sxs-lookup"><span data-stu-id="65253-147">String</span></span>|<span data-ttu-id="65253-148">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="65253-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="65253-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="65253-149">secureBoot</span></span>|<span data-ttu-id="65253-150">String</span><span class="sxs-lookup"><span data-stu-id="65253-150">String</span></span>|<span data-ttu-id="65253-151">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="65253-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="65253-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="65253-152">bootDebugging</span></span>|<span data-ttu-id="65253-153">String</span><span class="sxs-lookup"><span data-stu-id="65253-153">String</span></span>|<span data-ttu-id="65253-154">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="65253-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="65253-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="65253-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="65253-156">String</span><span class="sxs-lookup"><span data-stu-id="65253-156">String</span></span>|<span data-ttu-id="65253-157">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="65253-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="65253-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="65253-158">codeIntegrity</span></span>|<span data-ttu-id="65253-159">String</span><span class="sxs-lookup"><span data-stu-id="65253-159">String</span></span>| <span data-ttu-id="65253-160">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="65253-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="65253-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="65253-161">testSigning</span></span>|<span data-ttu-id="65253-162">String</span><span class="sxs-lookup"><span data-stu-id="65253-162">String</span></span>|<span data-ttu-id="65253-163">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="65253-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="65253-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="65253-164">safeMode</span></span>|<span data-ttu-id="65253-165">String</span><span class="sxs-lookup"><span data-stu-id="65253-165">String</span></span>|<span data-ttu-id="65253-166">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="65253-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="65253-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="65253-167">windowsPE</span></span>|<span data-ttu-id="65253-168">String</span><span class="sxs-lookup"><span data-stu-id="65253-168">String</span></span>|<span data-ttu-id="65253-169">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="65253-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="65253-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="65253-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="65253-171">String</span><span class="sxs-lookup"><span data-stu-id="65253-171">String</span></span>|<span data-ttu-id="65253-172">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="65253-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="65253-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="65253-173">virtualSecureMode</span></span>|<span data-ttu-id="65253-174">String</span><span class="sxs-lookup"><span data-stu-id="65253-174">String</span></span>|<span data-ttu-id="65253-175">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="65253-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="65253-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="65253-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="65253-177">String</span><span class="sxs-lookup"><span data-stu-id="65253-177">String</span></span>|<span data-ttu-id="65253-178">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="65253-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="65253-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="65253-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="65253-180">String</span><span class="sxs-lookup"><span data-stu-id="65253-180">String</span></span>|<span data-ttu-id="65253-181">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="65253-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="65253-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="65253-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="65253-183">String</span><span class="sxs-lookup"><span data-stu-id="65253-183">String</span></span>|<span data-ttu-id="65253-184">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="65253-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="65253-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="65253-185">tpmVersion</span></span>|<span data-ttu-id="65253-186">String</span><span class="sxs-lookup"><span data-stu-id="65253-186">String</span></span>|<span data-ttu-id="65253-187">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="65253-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="65253-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="65253-188">pcr0</span></span>|<span data-ttu-id="65253-189">String</span><span class="sxs-lookup"><span data-stu-id="65253-189">String</span></span>|<span data-ttu-id="65253-190">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="65253-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="65253-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="65253-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="65253-192">String</span><span class="sxs-lookup"><span data-stu-id="65253-192">String</span></span>|<span data-ttu-id="65253-193">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="65253-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="65253-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="65253-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="65253-195">String</span><span class="sxs-lookup"><span data-stu-id="65253-195">String</span></span>|<span data-ttu-id="65253-196">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="65253-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="65253-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="65253-197">bootRevisionListInfo</span></span>|<span data-ttu-id="65253-198">String</span><span class="sxs-lookup"><span data-stu-id="65253-198">String</span></span>|<span data-ttu-id="65253-199">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="65253-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="65253-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="65253-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="65253-201">String</span><span class="sxs-lookup"><span data-stu-id="65253-201">String</span></span>|<span data-ttu-id="65253-202">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="65253-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="65253-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="65253-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="65253-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65253-204">String</span></span>|<span data-ttu-id="65253-205">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="65253-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="65253-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="65253-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="65253-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65253-207">String</span></span>|<span data-ttu-id="65253-208">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="65253-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="65253-209">Relações</span><span class="sxs-lookup"><span data-stu-id="65253-209">Relationships</span></span>
<span data-ttu-id="65253-210">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65253-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65253-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65253-211">JSON Representation</span></span>
<span data-ttu-id="65253-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65253-212">Here is a JSON representation of the resource.</span></span>
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





