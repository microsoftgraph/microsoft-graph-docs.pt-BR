---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d56cc2689a9987f99ac7abd7a132ff1526bf88c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532215"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="12de5-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="12de5-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="12de5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12de5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12de5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12de5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12de5-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12de5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="12de5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12de5-107">Properties</span></span>
|<span data-ttu-id="12de5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12de5-108">Property</span></span>|<span data-ttu-id="12de5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12de5-109">Type</span></span>|<span data-ttu-id="12de5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12de5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12de5-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="12de5-111">lastUpdateDateTime</span></span>|<span data-ttu-id="12de5-112">String</span><span class="sxs-lookup"><span data-stu-id="12de5-112">String</span></span>|<span data-ttu-id="12de5-113">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="12de5-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="12de5-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="12de5-114">contentNamespaceUrl</span></span>|<span data-ttu-id="12de5-115">String</span><span class="sxs-lookup"><span data-stu-id="12de5-115">String</span></span>|<span data-ttu-id="12de5-116">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="12de5-116">The DHA report version.</span></span> <span data-ttu-id="12de5-117">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="12de5-117">(Namespace version)</span></span>|
|<span data-ttu-id="12de5-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="12de5-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="12de5-119">String</span><span class="sxs-lookup"><span data-stu-id="12de5-119">String</span></span>|<span data-ttu-id="12de5-120">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="12de5-120">The DHA report version.</span></span> <span data-ttu-id="12de5-121">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="12de5-121">(Namespace version)</span></span>|
|<span data-ttu-id="12de5-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="12de5-122">contentVersion</span></span>|<span data-ttu-id="12de5-123">String</span><span class="sxs-lookup"><span data-stu-id="12de5-123">String</span></span>|<span data-ttu-id="12de5-124">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="12de5-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="12de5-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="12de5-125">issuedDateTime</span></span>|<span data-ttu-id="12de5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12de5-126">DateTimeOffset</span></span>|<span data-ttu-id="12de5-127">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="12de5-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="12de5-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="12de5-128">attestationIdentityKey</span></span>|<span data-ttu-id="12de5-129">String</span><span class="sxs-lookup"><span data-stu-id="12de5-129">String</span></span>|<span data-ttu-id="12de5-130">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="12de5-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="12de5-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="12de5-131">resetCount</span></span>|<span data-ttu-id="12de5-132">Int64</span><span class="sxs-lookup"><span data-stu-id="12de5-132">Int64</span></span>|<span data-ttu-id="12de5-133">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="12de5-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="12de5-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="12de5-134">restartCount</span></span>|<span data-ttu-id="12de5-135">Int64</span><span class="sxs-lookup"><span data-stu-id="12de5-135">Int64</span></span>|<span data-ttu-id="12de5-136">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="12de5-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="12de5-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="12de5-137">dataExcutionPolicy</span></span>|<span data-ttu-id="12de5-138">String</span><span class="sxs-lookup"><span data-stu-id="12de5-138">String</span></span>|<span data-ttu-id="12de5-139">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="12de5-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="12de5-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="12de5-140">bitLockerStatus</span></span>|<span data-ttu-id="12de5-141">String</span><span class="sxs-lookup"><span data-stu-id="12de5-141">String</span></span>|<span data-ttu-id="12de5-142">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="12de5-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="12de5-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="12de5-143">bootManagerVersion</span></span>|<span data-ttu-id="12de5-144">String</span><span class="sxs-lookup"><span data-stu-id="12de5-144">String</span></span>|<span data-ttu-id="12de5-145">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="12de5-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="12de5-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="12de5-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="12de5-147">String</span><span class="sxs-lookup"><span data-stu-id="12de5-147">String</span></span>|<span data-ttu-id="12de5-148">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="12de5-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="12de5-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="12de5-149">secureBoot</span></span>|<span data-ttu-id="12de5-150">String</span><span class="sxs-lookup"><span data-stu-id="12de5-150">String</span></span>|<span data-ttu-id="12de5-151">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="12de5-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="12de5-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="12de5-152">bootDebugging</span></span>|<span data-ttu-id="12de5-153">String</span><span class="sxs-lookup"><span data-stu-id="12de5-153">String</span></span>|<span data-ttu-id="12de5-154">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="12de5-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="12de5-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="12de5-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="12de5-156">String</span><span class="sxs-lookup"><span data-stu-id="12de5-156">String</span></span>|<span data-ttu-id="12de5-157">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="12de5-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="12de5-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="12de5-158">codeIntegrity</span></span>|<span data-ttu-id="12de5-159">String</span><span class="sxs-lookup"><span data-stu-id="12de5-159">String</span></span>| <span data-ttu-id="12de5-160">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="12de5-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="12de5-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="12de5-161">testSigning</span></span>|<span data-ttu-id="12de5-162">String</span><span class="sxs-lookup"><span data-stu-id="12de5-162">String</span></span>|<span data-ttu-id="12de5-163">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="12de5-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="12de5-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="12de5-164">safeMode</span></span>|<span data-ttu-id="12de5-165">String</span><span class="sxs-lookup"><span data-stu-id="12de5-165">String</span></span>|<span data-ttu-id="12de5-166">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="12de5-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="12de5-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="12de5-167">windowsPE</span></span>|<span data-ttu-id="12de5-168">String</span><span class="sxs-lookup"><span data-stu-id="12de5-168">String</span></span>|<span data-ttu-id="12de5-169">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="12de5-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="12de5-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="12de5-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="12de5-171">String</span><span class="sxs-lookup"><span data-stu-id="12de5-171">String</span></span>|<span data-ttu-id="12de5-172">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="12de5-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="12de5-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="12de5-173">virtualSecureMode</span></span>|<span data-ttu-id="12de5-174">String</span><span class="sxs-lookup"><span data-stu-id="12de5-174">String</span></span>|<span data-ttu-id="12de5-175">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="12de5-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="12de5-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="12de5-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="12de5-177">String</span><span class="sxs-lookup"><span data-stu-id="12de5-177">String</span></span>|<span data-ttu-id="12de5-178">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="12de5-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="12de5-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="12de5-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="12de5-180">String</span><span class="sxs-lookup"><span data-stu-id="12de5-180">String</span></span>|<span data-ttu-id="12de5-181">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="12de5-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="12de5-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="12de5-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="12de5-183">String</span><span class="sxs-lookup"><span data-stu-id="12de5-183">String</span></span>|<span data-ttu-id="12de5-184">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="12de5-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="12de5-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="12de5-185">tpmVersion</span></span>|<span data-ttu-id="12de5-186">String</span><span class="sxs-lookup"><span data-stu-id="12de5-186">String</span></span>|<span data-ttu-id="12de5-187">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="12de5-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="12de5-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="12de5-188">pcr0</span></span>|<span data-ttu-id="12de5-189">String</span><span class="sxs-lookup"><span data-stu-id="12de5-189">String</span></span>|<span data-ttu-id="12de5-190">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="12de5-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="12de5-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="12de5-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="12de5-192">String</span><span class="sxs-lookup"><span data-stu-id="12de5-192">String</span></span>|<span data-ttu-id="12de5-193">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="12de5-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="12de5-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="12de5-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="12de5-195">String</span><span class="sxs-lookup"><span data-stu-id="12de5-195">String</span></span>|<span data-ttu-id="12de5-196">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="12de5-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="12de5-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="12de5-197">bootRevisionListInfo</span></span>|<span data-ttu-id="12de5-198">String</span><span class="sxs-lookup"><span data-stu-id="12de5-198">String</span></span>|<span data-ttu-id="12de5-199">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="12de5-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="12de5-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="12de5-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="12de5-201">String</span><span class="sxs-lookup"><span data-stu-id="12de5-201">String</span></span>|<span data-ttu-id="12de5-202">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="12de5-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="12de5-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="12de5-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="12de5-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12de5-204">String</span></span>|<span data-ttu-id="12de5-205">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="12de5-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="12de5-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="12de5-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="12de5-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12de5-207">String</span></span>|<span data-ttu-id="12de5-208">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="12de5-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="12de5-209">Relações</span><span class="sxs-lookup"><span data-stu-id="12de5-209">Relationships</span></span>
<span data-ttu-id="12de5-210">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12de5-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12de5-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12de5-211">JSON Representation</span></span>
<span data-ttu-id="12de5-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12de5-212">Here is a JSON representation of the resource.</span></span>
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




