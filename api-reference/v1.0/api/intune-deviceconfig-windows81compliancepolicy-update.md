---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3df5726032f7139f130ab8cf8366b9cdb497f6b
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732041"
---
# <a name="update-windows81compliancepolicy"></a>Atualizar windows81CompliancePolicy

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).

A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|passwordRequired|Booliano|Exige uma senha para desbloquear o dispositivo Windows.|
|passwordBlockSimple|Booliano|Indica se a senha simples deve ou não ser bloqueada.|
|passwordExpirationDays|Int32|Expiração da senha em dias.|
|passwordMinimumLength|Int32|Comprimento mínimo da senha.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 24|
|osMinimumVersion|Cadeia de caracteres|Versão mínima do Windows 8.1.|
|osMaximumVersion|Cadeia de caracteres|Versão máxima do Windows 8.1.|
|storageRequireEncryption|Booliano|Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





