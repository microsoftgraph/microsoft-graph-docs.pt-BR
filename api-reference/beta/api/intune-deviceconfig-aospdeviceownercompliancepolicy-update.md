---
title: Atualizar aospDeviceOwnerCompliancePolicy
description: Atualize as propriedades de um objeto aospDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7a90ab0d19a6dba44a42b653556c71b01e2011c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665672"
---
# <a name="update-aospdeviceownercompliancepolicy"></a>Atualizar aospDeviceOwnerCompliancePolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
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
No corpo da solicitação, fornece uma representação JSON para o [objeto aospDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|id|String|Chave da entidade. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)|
|osMinimumVersion|String|Versão mínima do Android.|
|osMaximumVersion|String|Versão máxima do Android.|
|minAndroidSecurityPatchLevel|String|Nível mínimo de patch de segurança Android.|
|passwordRequired|Boolean|Exige uma senha para desbloquear o dispositivo.|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Tipo de caracteres em senha. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária. Valores válidos de 1 a 8640|
|passwordMinimumLength|Int32|Comprimento mínimo da senha. Valores válidos de 4 a 16|
|storageRequireEncryption|Boolean|Exige criptografia em dispositivos Android.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto aospDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-aospdeviceownercompliancepolicy.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 593

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 765

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "0837b942-b942-0837-42b9-370842b93708",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumLength": 5,
  "storageRequireEncryption": true
}
```




