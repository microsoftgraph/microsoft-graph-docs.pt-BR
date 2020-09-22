---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a4e9b7e916f33bc6c472c5c90bd440a246f7016
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091198"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="fff86-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="fff86-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="fff86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fff86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fff86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fff86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fff86-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fff86-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fff86-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fff86-107">Properties</span></span>
|<span data-ttu-id="fff86-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fff86-108">Property</span></span>|<span data-ttu-id="fff86-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fff86-109">Type</span></span>|<span data-ttu-id="fff86-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fff86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fff86-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fff86-111">lastUpdateDateTime</span></span>|<span data-ttu-id="fff86-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-112">String</span></span>|<span data-ttu-id="fff86-113">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="fff86-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="fff86-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="fff86-114">contentNamespaceUrl</span></span>|<span data-ttu-id="fff86-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-115">String</span></span>|<span data-ttu-id="fff86-116">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="fff86-116">The DHA report version.</span></span> <span data-ttu-id="fff86-117">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="fff86-117">(Namespace version)</span></span>|
|<span data-ttu-id="fff86-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="fff86-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="fff86-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-119">String</span></span>|<span data-ttu-id="fff86-120">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="fff86-120">The DHA report version.</span></span> <span data-ttu-id="fff86-121">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="fff86-121">(Namespace version)</span></span>|
|<span data-ttu-id="fff86-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="fff86-122">contentVersion</span></span>|<span data-ttu-id="fff86-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-123">String</span></span>|<span data-ttu-id="fff86-124">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="fff86-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="fff86-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="fff86-125">issuedDateTime</span></span>|<span data-ttu-id="fff86-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fff86-126">DateTimeOffset</span></span>|<span data-ttu-id="fff86-127">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="fff86-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="fff86-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="fff86-128">attestationIdentityKey</span></span>|<span data-ttu-id="fff86-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-129">String</span></span>|<span data-ttu-id="fff86-130">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="fff86-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="fff86-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="fff86-131">resetCount</span></span>|<span data-ttu-id="fff86-132">Int64</span><span class="sxs-lookup"><span data-stu-id="fff86-132">Int64</span></span>|<span data-ttu-id="fff86-133">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="fff86-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="fff86-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="fff86-134">restartCount</span></span>|<span data-ttu-id="fff86-135">Int64</span><span class="sxs-lookup"><span data-stu-id="fff86-135">Int64</span></span>|<span data-ttu-id="fff86-136">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="fff86-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="fff86-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="fff86-137">dataExcutionPolicy</span></span>|<span data-ttu-id="fff86-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-138">String</span></span>|<span data-ttu-id="fff86-139">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="fff86-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="fff86-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="fff86-140">bitLockerStatus</span></span>|<span data-ttu-id="fff86-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-141">String</span></span>|<span data-ttu-id="fff86-142">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="fff86-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="fff86-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="fff86-143">bootManagerVersion</span></span>|<span data-ttu-id="fff86-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-144">String</span></span>|<span data-ttu-id="fff86-145">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="fff86-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="fff86-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="fff86-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="fff86-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-147">String</span></span>|<span data-ttu-id="fff86-148">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="fff86-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="fff86-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="fff86-149">secureBoot</span></span>|<span data-ttu-id="fff86-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-150">String</span></span>|<span data-ttu-id="fff86-151">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="fff86-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="fff86-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="fff86-152">bootDebugging</span></span>|<span data-ttu-id="fff86-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-153">String</span></span>|<span data-ttu-id="fff86-154">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="fff86-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="fff86-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="fff86-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="fff86-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-156">String</span></span>|<span data-ttu-id="fff86-157">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="fff86-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="fff86-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="fff86-158">codeIntegrity</span></span>|<span data-ttu-id="fff86-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-159">String</span></span>| <span data-ttu-id="fff86-160">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="fff86-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="fff86-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="fff86-161">testSigning</span></span>|<span data-ttu-id="fff86-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-162">String</span></span>|<span data-ttu-id="fff86-163">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="fff86-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="fff86-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="fff86-164">safeMode</span></span>|<span data-ttu-id="fff86-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-165">String</span></span>|<span data-ttu-id="fff86-166">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="fff86-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="fff86-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="fff86-167">windowsPE</span></span>|<span data-ttu-id="fff86-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-168">String</span></span>|<span data-ttu-id="fff86-169">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="fff86-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="fff86-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="fff86-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="fff86-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-171">String</span></span>|<span data-ttu-id="fff86-172">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="fff86-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="fff86-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="fff86-173">virtualSecureMode</span></span>|<span data-ttu-id="fff86-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-174">String</span></span>|<span data-ttu-id="fff86-175">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="fff86-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="fff86-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="fff86-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="fff86-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-177">String</span></span>|<span data-ttu-id="fff86-178">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="fff86-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="fff86-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="fff86-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="fff86-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-180">String</span></span>|<span data-ttu-id="fff86-181">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="fff86-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="fff86-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="fff86-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="fff86-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-183">String</span></span>|<span data-ttu-id="fff86-184">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="fff86-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="fff86-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="fff86-185">tpmVersion</span></span>|<span data-ttu-id="fff86-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-186">String</span></span>|<span data-ttu-id="fff86-187">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="fff86-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="fff86-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="fff86-188">pcr0</span></span>|<span data-ttu-id="fff86-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-189">String</span></span>|<span data-ttu-id="fff86-190">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="fff86-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="fff86-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="fff86-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="fff86-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-192">String</span></span>|<span data-ttu-id="fff86-193">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="fff86-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="fff86-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="fff86-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="fff86-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-195">String</span></span>|<span data-ttu-id="fff86-196">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="fff86-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="fff86-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="fff86-197">bootRevisionListInfo</span></span>|<span data-ttu-id="fff86-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-198">String</span></span>|<span data-ttu-id="fff86-199">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="fff86-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="fff86-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="fff86-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="fff86-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-201">String</span></span>|<span data-ttu-id="fff86-202">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="fff86-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="fff86-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="fff86-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="fff86-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-204">String</span></span>|<span data-ttu-id="fff86-205">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="fff86-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="fff86-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="fff86-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="fff86-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff86-207">String</span></span>|<span data-ttu-id="fff86-208">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="fff86-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="fff86-209">Relações</span><span class="sxs-lookup"><span data-stu-id="fff86-209">Relationships</span></span>
<span data-ttu-id="fff86-210">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fff86-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fff86-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fff86-211">JSON Representation</span></span>
<span data-ttu-id="fff86-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fff86-212">Here is a JSON representation of the resource.</span></span>
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









