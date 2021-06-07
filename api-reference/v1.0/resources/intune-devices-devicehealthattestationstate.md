---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89a8c990802a63bf72f36499e222321f83a0dade
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755018"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="b5f17-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="b5f17-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="b5f17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5f17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5f17-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5f17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5f17-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b5f17-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b5f17-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5f17-107">Properties</span></span>
|<span data-ttu-id="b5f17-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5f17-108">Property</span></span>|<span data-ttu-id="b5f17-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5f17-109">Type</span></span>|<span data-ttu-id="b5f17-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5f17-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b5f17-111">lastUpdateDateTime</span></span>|<span data-ttu-id="b5f17-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-112">String</span></span>|<span data-ttu-id="b5f17-113">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="b5f17-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="b5f17-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="b5f17-114">contentNamespaceUrl</span></span>|<span data-ttu-id="b5f17-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-115">String</span></span>|<span data-ttu-id="b5f17-116">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="b5f17-116">The DHA report version.</span></span> <span data-ttu-id="b5f17-117">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="b5f17-117">(Namespace version)</span></span>|
|<span data-ttu-id="b5f17-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="b5f17-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="b5f17-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-119">String</span></span>|<span data-ttu-id="b5f17-120">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="b5f17-120">The DHA report version.</span></span> <span data-ttu-id="b5f17-121">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="b5f17-121">(Namespace version)</span></span>|
|<span data-ttu-id="b5f17-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="b5f17-122">contentVersion</span></span>|<span data-ttu-id="b5f17-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-123">String</span></span>|<span data-ttu-id="b5f17-124">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="b5f17-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="b5f17-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5f17-125">issuedDateTime</span></span>|<span data-ttu-id="b5f17-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5f17-126">DateTimeOffset</span></span>|<span data-ttu-id="b5f17-127">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="b5f17-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="b5f17-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="b5f17-128">attestationIdentityKey</span></span>|<span data-ttu-id="b5f17-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-129">String</span></span>|<span data-ttu-id="b5f17-130">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="b5f17-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="b5f17-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="b5f17-131">resetCount</span></span>|<span data-ttu-id="b5f17-132">Int64</span><span class="sxs-lookup"><span data-stu-id="b5f17-132">Int64</span></span>|<span data-ttu-id="b5f17-133">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="b5f17-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="b5f17-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="b5f17-134">restartCount</span></span>|<span data-ttu-id="b5f17-135">Int64</span><span class="sxs-lookup"><span data-stu-id="b5f17-135">Int64</span></span>|<span data-ttu-id="b5f17-136">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="b5f17-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="b5f17-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="b5f17-137">dataExcutionPolicy</span></span>|<span data-ttu-id="b5f17-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-138">String</span></span>|<span data-ttu-id="b5f17-139">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="b5f17-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="b5f17-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="b5f17-140">bitLockerStatus</span></span>|<span data-ttu-id="b5f17-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-141">String</span></span>|<span data-ttu-id="b5f17-142">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="b5f17-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="b5f17-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="b5f17-143">bootManagerVersion</span></span>|<span data-ttu-id="b5f17-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-144">String</span></span>|<span data-ttu-id="b5f17-145">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="b5f17-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="b5f17-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="b5f17-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="b5f17-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-147">String</span></span>|<span data-ttu-id="b5f17-148">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="b5f17-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="b5f17-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="b5f17-149">secureBoot</span></span>|<span data-ttu-id="b5f17-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-150">String</span></span>|<span data-ttu-id="b5f17-151">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="b5f17-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="b5f17-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="b5f17-152">bootDebugging</span></span>|<span data-ttu-id="b5f17-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-153">String</span></span>|<span data-ttu-id="b5f17-154">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="b5f17-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="b5f17-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="b5f17-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="b5f17-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-156">String</span></span>|<span data-ttu-id="b5f17-157">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="b5f17-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="b5f17-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="b5f17-158">codeIntegrity</span></span>|<span data-ttu-id="b5f17-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-159">String</span></span>| <span data-ttu-id="b5f17-160">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="b5f17-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="b5f17-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="b5f17-161">testSigning</span></span>|<span data-ttu-id="b5f17-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-162">String</span></span>|<span data-ttu-id="b5f17-163">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="b5f17-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="b5f17-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="b5f17-164">safeMode</span></span>|<span data-ttu-id="b5f17-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-165">String</span></span>|<span data-ttu-id="b5f17-166">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="b5f17-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="b5f17-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="b5f17-167">windowsPE</span></span>|<span data-ttu-id="b5f17-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-168">String</span></span>|<span data-ttu-id="b5f17-169">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="b5f17-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="b5f17-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="b5f17-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="b5f17-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-171">String</span></span>|<span data-ttu-id="b5f17-172">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="b5f17-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="b5f17-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="b5f17-173">virtualSecureMode</span></span>|<span data-ttu-id="b5f17-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-174">String</span></span>|<span data-ttu-id="b5f17-175">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="b5f17-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="b5f17-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b5f17-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="b5f17-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-177">String</span></span>|<span data-ttu-id="b5f17-178">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="b5f17-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="b5f17-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="b5f17-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="b5f17-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-180">String</span></span>|<span data-ttu-id="b5f17-181">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="b5f17-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="b5f17-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="b5f17-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="b5f17-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-183">String</span></span>|<span data-ttu-id="b5f17-184">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="b5f17-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="b5f17-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="b5f17-185">tpmVersion</span></span>|<span data-ttu-id="b5f17-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-186">String</span></span>|<span data-ttu-id="b5f17-187">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="b5f17-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="b5f17-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="b5f17-188">pcr0</span></span>|<span data-ttu-id="b5f17-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-189">String</span></span>|<span data-ttu-id="b5f17-190">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="b5f17-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="b5f17-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="b5f17-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="b5f17-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-192">String</span></span>|<span data-ttu-id="b5f17-193">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="b5f17-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="b5f17-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="b5f17-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="b5f17-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-195">String</span></span>|<span data-ttu-id="b5f17-196">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="b5f17-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="b5f17-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="b5f17-197">bootRevisionListInfo</span></span>|<span data-ttu-id="b5f17-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-198">String</span></span>|<span data-ttu-id="b5f17-199">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="b5f17-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="b5f17-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="b5f17-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="b5f17-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-201">String</span></span>|<span data-ttu-id="b5f17-202">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="b5f17-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="b5f17-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="b5f17-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="b5f17-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-204">String</span></span>|<span data-ttu-id="b5f17-205">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="b5f17-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="b5f17-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="b5f17-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="b5f17-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5f17-207">String</span></span>|<span data-ttu-id="b5f17-208">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="b5f17-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5f17-209">Relações</span><span class="sxs-lookup"><span data-stu-id="b5f17-209">Relationships</span></span>
<span data-ttu-id="b5f17-210">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b5f17-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5f17-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5f17-211">JSON Representation</span></span>
<span data-ttu-id="b5f17-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5f17-212">Here is a JSON representation of the resource.</span></span>
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




