---
title: 'informationProtectionLabel: evaluateRemoval'
description: Avaliar qual rótulo remover e como removê-lo com base nas informações de conteúdo existentes.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5d8723285ab364d7453d782806064e12de2b78f5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938538"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="01fa7-103">informationProtectionLabel: evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="01fa7-103">informationProtectionLabel: evaluateRemoval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01fa7-104">Indique o aplicativo de consumo que ações deve executar para remover as informações de rótulo.</span><span class="sxs-lookup"><span data-stu-id="01fa7-104">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="01fa7-105">Dada [contentInfo](../resources/contentinfo.md) como uma entrada, que inclui [pares de chave/valor](../resources/keyvaluepair.md)de metadados de conteúdo existentes, a API retorna um [informationProtectionAction](../resources/informationprotectionaction.md) que contém alguma combinação de uma ou mais das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="01fa7-105">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="01fa7-106">justifyaction</span><span class="sxs-lookup"><span data-stu-id="01fa7-106">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="01fa7-107">metadataaction</span><span class="sxs-lookup"><span data-stu-id="01fa7-107">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="01fa7-108">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="01fa7-108">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="01fa7-109">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="01fa7-109">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="01fa7-110">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="01fa7-110">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="01fa7-111">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="01fa7-111">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="01fa7-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="01fa7-112">Permissions</span></span>

<span data-ttu-id="01fa7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01fa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01fa7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01fa7-115">Permission type</span></span>                        | <span data-ttu-id="01fa7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01fa7-116">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="01fa7-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01fa7-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="01fa7-118">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="01fa7-118">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="01fa7-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01fa7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01fa7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01fa7-120">Not supported.</span></span>                              |
| <span data-ttu-id="01fa7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01fa7-121">Application</span></span>                            | <span data-ttu-id="01fa7-122">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="01fa7-122">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="01fa7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01fa7-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="01fa7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01fa7-124">Request headers</span></span>

| <span data-ttu-id="01fa7-125">Nome</span><span class="sxs-lookup"><span data-stu-id="01fa7-125">Name</span></span>          | <span data-ttu-id="01fa7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="01fa7-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="01fa7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="01fa7-127">Authorization</span></span> | <span data-ttu-id="01fa7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01fa7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="01fa7-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="01fa7-130">Content-type</span></span>  | <span data-ttu-id="01fa7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01fa7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01fa7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01fa7-133">Request body</span></span>

<span data-ttu-id="01fa7-134">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01fa7-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01fa7-135">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="01fa7-135">Parameter</span></span>              | <span data-ttu-id="01fa7-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="01fa7-136">Type</span></span>                                                             | <span data-ttu-id="01fa7-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="01fa7-137">Description</span></span>                                                                                                                                                                                                   |
| :--------------------- | :--------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="01fa7-138">contentInfo</span><span class="sxs-lookup"><span data-stu-id="01fa7-138">contentInfo</span></span>            | [<span data-ttu-id="01fa7-139">contentInfo</span><span class="sxs-lookup"><span data-stu-id="01fa7-139">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="01fa7-140">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="01fa7-140">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="01fa7-141">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="01fa7-141">downgradeJustification</span></span> | [<span data-ttu-id="01fa7-142">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="01fa7-142">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="01fa7-143">Justificativa que deve ser fornecida pelo usuário ou pela lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="01fa7-143">Justification that must be provided by the user or application logic.</span></span>                                                                                                                                         |


## <a name="response"></a><span data-ttu-id="01fa7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="01fa7-144">Response</span></span>

<span data-ttu-id="01fa7-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [informationProtectionAction](../resources/informationprotectionaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01fa7-145">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="01fa7-146">O [objeto informationProtectionAction](../resources/informationprotectionaction.md) conterá um objeto [metadataaction](../resources/metadataaction.md) que informa ao aplicativo quais metadados serão removidos.</span><span class="sxs-lookup"><span data-stu-id="01fa7-146">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="01fa7-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="01fa7-147">Examples</span></span>

<span data-ttu-id="01fa7-148">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="01fa7-148">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="01fa7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01fa7-149">Request</span></span>

<span data-ttu-id="01fa7-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01fa7-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateRemoval
Content-type: application/json

{
  "contentInfo": {
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "format": "default",
    "identifier": null,
    "state@odata.type": "#microsoft.graph.contentState",
    "state": "rest",
    "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
    "metadata": [
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
        "value": "True"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
        "value": "Standard"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
        "value": "1/1/0001 12:00:00 AM"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
        "value": "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
        "value": "General"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
        "value": "0"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
        "value": "00000000-0000-0000-0000-000000000000"
      }
    ]
  },
  "downgradeJustification": {
        "justificationMessage": "The information has been declassified.",
        "isDowngradeJustified": true
    }
}
```

### <a name="response"></a><span data-ttu-id="01fa7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="01fa7-151">Response</span></span>

<span data-ttu-id="01fa7-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01fa7-152">The following is an example of the response.</span></span>

> <span data-ttu-id="01fa7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01fa7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "@odata.type": "#microsoft.graph.metadataAction",
            "metadataToRemove": [
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
            ],
            "metadataToAdd": []
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateRemoval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
