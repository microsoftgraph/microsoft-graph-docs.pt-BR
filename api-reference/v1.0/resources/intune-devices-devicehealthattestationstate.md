---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53fa5cdafdc125fdc32ef599a625c58e3bcbe687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563809"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="390d0-103">Tipo de recurso deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="390d0-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="390d0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="390d0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="390d0-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="390d0-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="390d0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="390d0-106">Properties</span></span>
|<span data-ttu-id="390d0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="390d0-107">Property</span></span>|<span data-ttu-id="390d0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="390d0-108">Type</span></span>|<span data-ttu-id="390d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="390d0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="390d0-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="390d0-110">lastUpdateDateTime</span></span>|<span data-ttu-id="390d0-111">String</span><span class="sxs-lookup"><span data-stu-id="390d0-111">String</span></span>|<span data-ttu-id="390d0-112">Carimbo de data/hora da última atualização.</span><span class="sxs-lookup"><span data-stu-id="390d0-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="390d0-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="390d0-113">contentNamespaceUrl</span></span>|<span data-ttu-id="390d0-114">String</span><span class="sxs-lookup"><span data-stu-id="390d0-114">String</span></span>|<span data-ttu-id="390d0-115">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="390d0-115">The DHA report version.</span></span> <span data-ttu-id="390d0-116">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="390d0-116">(Namespace version)</span></span>|
|<span data-ttu-id="390d0-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="390d0-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="390d0-118">String</span><span class="sxs-lookup"><span data-stu-id="390d0-118">String</span></span>|<span data-ttu-id="390d0-119">A versão do relatório DHA.</span><span class="sxs-lookup"><span data-stu-id="390d0-119">The DHA report version.</span></span> <span data-ttu-id="390d0-120">(Versão NameSpace)</span><span class="sxs-lookup"><span data-stu-id="390d0-120">(Namespace version)</span></span>|
|<span data-ttu-id="390d0-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="390d0-121">contentVersion</span></span>|<span data-ttu-id="390d0-122">String</span><span class="sxs-lookup"><span data-stu-id="390d0-122">String</span></span>|<span data-ttu-id="390d0-123">Versão do esquema do estado HealthAttestation</span><span class="sxs-lookup"><span data-stu-id="390d0-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="390d0-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="390d0-124">issuedDateTime</span></span>|<span data-ttu-id="390d0-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="390d0-125">DateTimeOffset</span></span>|<span data-ttu-id="390d0-126">Data e hora em que o dispositivo foi avaliado ou emitido para o MDM</span><span class="sxs-lookup"><span data-stu-id="390d0-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="390d0-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="390d0-127">attestationIdentityKey</span></span>|<span data-ttu-id="390d0-128">String</span><span class="sxs-lookup"><span data-stu-id="390d0-128">String</span></span>|<span data-ttu-id="390d0-129">Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).</span><span class="sxs-lookup"><span data-stu-id="390d0-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="390d0-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="390d0-130">resetCount</span></span>|<span data-ttu-id="390d0-131">Int64</span><span class="sxs-lookup"><span data-stu-id="390d0-131">Int64</span></span>|<span data-ttu-id="390d0-132">Número de vezes que um dispositivo PC hibernou ou foi retomado</span><span class="sxs-lookup"><span data-stu-id="390d0-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="390d0-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="390d0-133">restartCount</span></span>|<span data-ttu-id="390d0-134">Int64</span><span class="sxs-lookup"><span data-stu-id="390d0-134">Int64</span></span>|<span data-ttu-id="390d0-135">Número de vezes que um dispositivo PC foi reiniciado</span><span class="sxs-lookup"><span data-stu-id="390d0-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="390d0-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="390d0-136">dataExcutionPolicy</span></span>|<span data-ttu-id="390d0-137">String</span><span class="sxs-lookup"><span data-stu-id="390d0-137">String</span></span>|<span data-ttu-id="390d0-138">A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória</span><span class="sxs-lookup"><span data-stu-id="390d0-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="390d0-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="390d0-139">bitLockerStatus</span></span>|<span data-ttu-id="390d0-140">String</span><span class="sxs-lookup"><span data-stu-id="390d0-140">String</span></span>|<span data-ttu-id="390d0-141">O status ativado ou desativado do BitLocker</span><span class="sxs-lookup"><span data-stu-id="390d0-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="390d0-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="390d0-142">bootManagerVersion</span></span>|<span data-ttu-id="390d0-143">String</span><span class="sxs-lookup"><span data-stu-id="390d0-143">String</span></span>|<span data-ttu-id="390d0-144">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="390d0-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="390d0-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="390d0-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="390d0-146">String</span><span class="sxs-lookup"><span data-stu-id="390d0-146">String</span></span>|<span data-ttu-id="390d0-147">A versão do Gerenciador de Inicialização.</span><span class="sxs-lookup"><span data-stu-id="390d0-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="390d0-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="390d0-148">secureBoot</span></span>|<span data-ttu-id="390d0-149">String</span><span class="sxs-lookup"><span data-stu-id="390d0-149">String</span></span>|<span data-ttu-id="390d0-150">Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas</span><span class="sxs-lookup"><span data-stu-id="390d0-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="390d0-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="390d0-151">bootDebugging</span></span>|<span data-ttu-id="390d0-152">String</span><span class="sxs-lookup"><span data-stu-id="390d0-152">String</span></span>|<span data-ttu-id="390d0-153">Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="390d0-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="390d0-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="390d0-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="390d0-155">String</span><span class="sxs-lookup"><span data-stu-id="390d0-155">String</span></span>|<span data-ttu-id="390d0-156">Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes</span><span class="sxs-lookup"><span data-stu-id="390d0-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="390d0-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="390d0-157">codeIntegrity</span></span>|<span data-ttu-id="390d0-158">String</span><span class="sxs-lookup"><span data-stu-id="390d0-158">String</span></span>| <span data-ttu-id="390d0-159">Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada</span><span class="sxs-lookup"><span data-stu-id="390d0-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="390d0-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="390d0-160">testSigning</span></span>|<span data-ttu-id="390d0-161">String</span><span class="sxs-lookup"><span data-stu-id="390d0-161">String</span></span>|<span data-ttu-id="390d0-162">Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização</span><span class="sxs-lookup"><span data-stu-id="390d0-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="390d0-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="390d0-163">safeMode</span></span>|<span data-ttu-id="390d0-164">String</span><span class="sxs-lookup"><span data-stu-id="390d0-164">String</span></span>|<span data-ttu-id="390d0-165">O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado</span><span class="sxs-lookup"><span data-stu-id="390d0-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="390d0-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="390d0-166">windowsPE</span></span>|<span data-ttu-id="390d0-167">String</span><span class="sxs-lookup"><span data-stu-id="390d0-167">String</span></span>|<span data-ttu-id="390d0-168">Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows</span><span class="sxs-lookup"><span data-stu-id="390d0-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="390d0-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="390d0-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="390d0-170">String</span><span class="sxs-lookup"><span data-stu-id="390d0-170">String</span></span>|<span data-ttu-id="390d0-171">ELAM fornece proteção aos computadores da sua rede quando eles são inicializados</span><span class="sxs-lookup"><span data-stu-id="390d0-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="390d0-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="390d0-172">virtualSecureMode</span></span>|<span data-ttu-id="390d0-173">String</span><span class="sxs-lookup"><span data-stu-id="390d0-173">String</span></span>|<span data-ttu-id="390d0-174">VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido</span><span class="sxs-lookup"><span data-stu-id="390d0-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="390d0-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="390d0-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="390d0-176">String</span><span class="sxs-lookup"><span data-stu-id="390d0-176">String</span></span>|<span data-ttu-id="390d0-177">Atributo informativo que identifica o algoritmo HASH usado por TPM</span><span class="sxs-lookup"><span data-stu-id="390d0-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="390d0-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="390d0-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="390d0-179">String</span><span class="sxs-lookup"><span data-stu-id="390d0-179">String</span></span>|<span data-ttu-id="390d0-180">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="390d0-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="390d0-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="390d0-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="390d0-182">String</span><span class="sxs-lookup"><span data-stu-id="390d0-182">String</span></span>|<span data-ttu-id="390d0-183">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="390d0-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="390d0-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="390d0-184">tpmVersion</span></span>|<span data-ttu-id="390d0-185">String</span><span class="sxs-lookup"><span data-stu-id="390d0-185">String</span></span>|<span data-ttu-id="390d0-186">O número de versão de segurança do Aplicativo de Inicialização</span><span class="sxs-lookup"><span data-stu-id="390d0-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="390d0-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="390d0-187">pcr0</span></span>|<span data-ttu-id="390d0-188">String</span><span class="sxs-lookup"><span data-stu-id="390d0-188">String</span></span>|<span data-ttu-id="390d0-189">A medida capturada no PCR\[0\]</span><span class="sxs-lookup"><span data-stu-id="390d0-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="390d0-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="390d0-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="390d0-191">String</span><span class="sxs-lookup"><span data-stu-id="390d0-191">String</span></span>|<span data-ttu-id="390d0-192">Impressão digital da política de configuração de Inicialização Segura personalizada</span><span class="sxs-lookup"><span data-stu-id="390d0-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="390d0-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="390d0-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="390d0-194">String</span><span class="sxs-lookup"><span data-stu-id="390d0-194">String</span></span>|<span data-ttu-id="390d0-195">A política de Integridade de código que está controlando a segurança do ambiente de inicialização</span><span class="sxs-lookup"><span data-stu-id="390d0-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="390d0-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="390d0-196">bootRevisionListInfo</span></span>|<span data-ttu-id="390d0-197">String</span><span class="sxs-lookup"><span data-stu-id="390d0-197">String</span></span>|<span data-ttu-id="390d0-198">A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="390d0-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="390d0-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="390d0-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="390d0-200">String</span><span class="sxs-lookup"><span data-stu-id="390d0-200">String</span></span>|<span data-ttu-id="390d0-201">A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado</span><span class="sxs-lookup"><span data-stu-id="390d0-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="390d0-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="390d0-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="390d0-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="390d0-203">String</span></span>|<span data-ttu-id="390d0-204">Esse atributo será exibido se o serviço DHA detectar um problema de integridade</span><span class="sxs-lookup"><span data-stu-id="390d0-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="390d0-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="390d0-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="390d0-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="390d0-206">String</span></span>|<span data-ttu-id="390d0-207">Esse atributo indica se DHA é compatível com o dispositivo</span><span class="sxs-lookup"><span data-stu-id="390d0-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="390d0-208">Relações</span><span class="sxs-lookup"><span data-stu-id="390d0-208">Relationships</span></span>
<span data-ttu-id="390d0-209">Nenhum</span><span class="sxs-lookup"><span data-stu-id="390d0-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="390d0-210">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="390d0-210">JSON Representation</span></span>
<span data-ttu-id="390d0-211">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="390d0-211">Here is a JSON representation of the resource.</span></span>
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



