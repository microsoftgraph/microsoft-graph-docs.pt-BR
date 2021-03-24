---
title: Atualizar termsAndConditionsGroupAssignment
description: Atualize as propriedades de um objeto termsAndConditionsGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 160091cfa2d9d5add4bab8ed3bd16301b90f4268
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132839"
---
# <a name="update-termsandconditionsgroupassignment"></a>Atualizar termsAndConditionsGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para [o objeto termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [os termosAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|targetGroupId|Cadeia de caracteres|Identificador exclusivo de um grupo ao&C atribuído.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




