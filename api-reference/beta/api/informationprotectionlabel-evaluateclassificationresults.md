---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: Avalie qual rótulo aplicar com base nas informações de conteúdo existentes e em um resultado de classificação.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 26c65411ba7ce83fdae9d6d5ac46038deea84ac3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004784"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a>informationProtectionLabel: evaluateClassificationResults

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usando [resultados de](../resources/classificationresult.md)classificação, calcule o rótulo de proteção de informações que deve ser aplicado e retorne o conjunto de ações que devem ser tomadas para rotular corretamente as informações. [](../resources/informationprotectionlabel.md) Essa API é útil quando um rótulo deve ser definido automaticamente com base na classificação do conteúdo do arquivo, em vez de rotulado diretamente por um usuário ou serviço. 

Para avaliar com base nos resultados da classificação, forneça [contentInfo](../resources/contentinfo.md), que inclui pares de [chave/valor](../resources/keyvaluepair.md)de metadados de conteúdo existentes e resultados [de classificação.](../resources/classificationresult.md) A API retorna [uma informationProtectionAction](../resources/informationprotectionaction.md) que contém um dos seguintes: 

* [addContentFooterAction](../resources/addcontentfooteraction.md)
* [addContentHeaderAction](../resources/addcontentheaderaction.md)
* [addWatermarkAction](../resources/addWatermarkaction.md)
* [applyLabelAction](../resources/applylabelaction.md)
* [customAction](../resources/customaction.md)
* [justifyAction](../resources/justifyaction.md)
* [metadataAction](../resources/metadataaction.md)
* [protectAdhocAction](../resources/protectadhocaction.md)
* [protectByTemplateAction](../resources/protectBytemplateaction.md)
* [protectionDoNotForwardAction](../resources/protectdonotforwardaction.md)
* [recommendLabelAction](../resources/recommendlabelaction.md)
* [removeContentFooterAction](../resources/removecontentfooteraction.md)
* [removeContentHeaderAction](../resources/removecontentheaderaction.md)
* [removeProtectionAction](../resources/removeprotectionaction.md)
* [removeWatermarkAction](../resources/removewatermarkaction.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | InformationProtectionPolicy. Read            |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | InformationProtectionPolicy.Read.All        |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autorização | {token} de portador. Obrigatório.                                                                                                                                             |
| Content-type  | application/json. Obrigatório.                                                                                                                                           |
| User-Agent    | Descreve o nome e a versão do aplicativo de chamada. Os detalhes aparecerão no Azure Information Protection Analytics. O formato sugerido é ApplicationName/Version. Opcional. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro             | Tipo                                                                    | Descrição                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| contentInfo           | [contentInfo](../resources/contentInfo.md)                              | Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.                                                                                                                                                   |
| classificationResults | [coleção classificationResult](../resources/classificationresult.md) | Contém o conjunto de resultados de classificação retornados pelo ponto de extremidade de classificação de dados. As informações de classificação são usadas para determinar o rótulo apropriado com base na configuração Proteção de Informações da Microsoft rótulo de política no Office 365 Centro de Conformidade e Segurança. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um novo objeto da coleção `200 OK` [informationProtectionAction](../resources/informationprotectionaction.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/evaluateClassificationResults
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "contentInfo": {
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "format": "default",
    "identifier": null,
    "state@odata.type": "#microsoft.graph.contentState",
    "state": "rest"
  },
  "classificationResults": [
    {
      "sensitiveTypeId": "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
      "count": 4,
      "confidenceLevel": 75
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-evaluateclassificationresults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/informationprotectionlabel-evaluateclassificationresults-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.informationProtectionAction)",
  "value": [
    {
      "@odata.type": "#microsoft.graph.applyLabelAction",
      "responsibleSensitiveTypeIds": [
        "cb353f78-2b72-4c3c-8827-92ebe4f69fdf"
      ],
      "actionSource": "automatic",
      "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is Top Secret.",
        "isActive": true
      },
      "actions": [
        {
          "@odata.type": "#microsoft.graph.protectByTemplateAction",
          "templateId": "0e7fea72-7bba-4438-a070-95c292cd6f8c"
        },
        {
          "@odata.type": "#microsoft.graph.metadataAction",
          "metadataToRemove": [],
          "metadataToAdd": [
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
              "value": "true"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
              "value": "2019-10-03T21:50:20Z"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
              "value": "Standard"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
              "value": "Top Secret"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
              "value": "cb46c030-1825-4e81-a295-151c039dbf02"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
              "value": "76dc494e-6c59-43e6-88a1-0000edd58fca"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
              "value": "8"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateClassificationResults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


