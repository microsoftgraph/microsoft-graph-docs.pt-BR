---
title: Atualizar deviceConfigurationUserStateSummary
description: Atualize as propriedades de um objeto deviceConfigurationUserStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f95ee2ccac6e200b8b3609e34ca66e768f305b828b2c3e88a2b37cd7681d6ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195957"
---
# <a name="update-deviceconfigurationuserstatesummary"></a>Atualizar deviceConfigurationUserStateSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)

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
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|unknownUserCount|Int32|Número de usuários desconhecidos|
|notApplicableUserCount|Int32|Número de usuários não aplicáveis|
|compliantUserCount|Int32|Número de usuários compatíveis|
|remediatedUserCount|Int32|Número de usuários remediados|
|nonCompliantUserCount|Int32|Número de usuários não compatíveis|
|errorUserCount|Int32|Número de usuários de erros|
|conflictUserCount|Int32|Número de usuários em conflito|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```




