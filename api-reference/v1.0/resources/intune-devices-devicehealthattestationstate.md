---
title: Tipo de recurso deviceHealthAttestationState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3d9b597853a22d167af8c41a7b41523163fa9a6
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445939"
---
# <a name="devicehealthattestationstate-resource-type"></a>Tipo de recurso deviceHealthAttestationState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastUpdateDateTime|Cadeia de caracteres|Carimbo de data/hora da última atualização.|
|contentNamespaceUrl|Cadeia de caracteres|A versão do relatório DHA. (Versão NameSpace)|
|deviceHealthAttestationStatus|Cadeia de caracteres|A versão do relatório DHA. (Versão NameSpace)|
|contentVersion|Cadeia de caracteres|Versão do esquema do estado HealthAttestation|
|issuedDateTime|DateTimeOffset|Data e hora em que o dispositivo foi avaliado ou emitido para o MDM|
|attestationIdentityKey|Cadeia de caracteres|Quando houver uma chave de identidade de atestado (AIK) em um dispositivo, isso indica que o dispositivo tem um certificado de chave de endosso (EK).|
|resetCount|Int64|Número de vezes que um dispositivo PC hibernou ou foi retomado|
|restartCount|Int64|Número de vezes que um dispositivo PC foi reiniciado|
|dataExcutionPolicy|Cadeia de caracteres|A Política de DEP define um conjunto de tecnologias de hardware e software que executa verificações adicionais na memória |
|bitLockerStatus|Cadeia de caracteres|O status ativado ou desativado do BitLocker|
|bootManagerVersion|Cadeia de caracteres|A versão do Gerenciador de Inicialização.|
|codeIntegrityCheckVersion|Cadeia de caracteres|A versão do Gerenciador de Inicialização.|
|secureBoot|Cadeia de caracteres|Quando a 	Inicialização Segura está habilitada, os principais componentes devem ter as assinaturas criptográficas corretas|
|bootDebugging|Cadeia de caracteres|Quando BootDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes|
|operatingSystemKernelDebugging|Cadeia de caracteres|Quando operatingSystemKernelDebugging está habilitado, o dispositivo é usado em desenvolvimentos e testes|
|codeIntegrity|Cadeia de caracteres| Quando a integridade de código está habilitada, a execução do código fica restrita a código com integridade verificada|
|testSigning|Cadeia de caracteres|Quando a assinatura de teste é permitida, o dispositivo não impõe a validação de assinatura durante a inicialização|
|safeMode|Cadeia de caracteres|O modo de segurança é uma opção de solução de problemas do Windows que inicia o computador em um estado limitado|
|windowsPE|Cadeia de caracteres|Sistema operacional executado com serviços limitados, usado para preparar um computador para o Windows|
|earlyLaunchAntiMalwareDriverProtection|Cadeia de caracteres|ELAM fornece proteção aos computadores da sua rede quando eles são inicializados|
|virtualSecureMode|Cadeia de caracteres|VSM é um contêiner que protege ativos de alto valor contra um kernel comprometido|
|pcrHashAlgorithm|Cadeia de caracteres|Atributo informativo que identifica o algoritmo HASH usado por TPM|
|bootAppSecurityVersion|Cadeia de caracteres|O número de versão de segurança do Aplicativo de Inicialização|
|bootManagerSecurityVersion|Cadeia de caracteres|O número de versão de segurança do Aplicativo de Inicialização|
|tpmVersion|Cadeia de caracteres|O número de versão de segurança do Aplicativo de Inicialização|
|pcr0|Cadeia de caracteres|A medida capturada no PCR\[0\]|
|secureBootConfigurationPolicyFingerPrint|Cadeia de caracteres|Impressão digital da política de configuração de Inicialização Segura personalizada|
|codeIntegrityPolicy|Cadeia de caracteres|A política de Integridade de código que está controlando a segurança do ambiente de inicialização|
|bootRevisionListInfo|Cadeia de caracteres|A Lista de revisão de inicialização carregada durante a inicialização inicial no dispositivo confirmado|
|operatingSystemRevListInfo|Cadeia de caracteres|A Lista de revisão de sistema operacional carregada durante a inicialização inicial no dispositivo confirmado|
|healthStatusMismatchInfo|Cadeia de caracteres|Esse atributo será exibido se o serviço DHA detectar um problema de integridade|
|healthAttestationSupportedStatus|Cadeia de caracteres|Esse atributo indica se DHA é compatível com o dispositivo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
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



