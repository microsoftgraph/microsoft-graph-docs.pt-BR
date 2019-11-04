---
title: 'informationProtectionLabel: evaluateApplication'
description: Avaliar qual rótulo aplicar com base nas informações de conteúdo existentes e no estado de conteúdo desejado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69dbbddf0529848e0f8ed8676b8556ff3e93edf8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938545"
---
# <a name="informationprotectionlabel-evaluateapplication"></a><span data-ttu-id="2d063-103">informationProtectionLabel: evaluateApplication</span><span class="sxs-lookup"><span data-stu-id="2d063-103">informationProtectionLabel: evaluateApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d063-104">Compute o [rótulo de proteção de informações](../resources/informationprotectionlabel.md) que deve ser aplicado e retornar o conjunto de ações que devem ser executadas para rotular corretamente as informações.</span><span class="sxs-lookup"><span data-stu-id="2d063-104">Compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="2d063-105">Essa API é útil quando um rótulo deve ser definido manualmente ou explicitamente por um usuário ou serviço, e não automaticamente com base no conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2d063-105">This API is useful when a label should be set manually or explicitly by a user or service, rather than automatically based on file contents.</span></span> 

<span data-ttu-id="2d063-106">Dada [contentInfo](../resources/contentInfo.md), que inclui [pares de chave/valor](../resources/keyvaluepair.md)de metadados de conteúdo existentes e [LABELINGOPTIONS](../resources/labelingoptions.md) como entrada, a API retorna um objeto [informationProtectionAction](../resources/informationprotectionaction.md) que contém uma ou mais das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="2d063-106">Given [contentInfo](../resources/contentInfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [labelingOptions](../resources/labelingoptions.md) as an input, the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) object that contains one of more of the following:</span></span> 

* [<span data-ttu-id="2d063-107">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2d063-107">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="2d063-108">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2d063-108">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="2d063-109">addwatermarkaction</span><span class="sxs-lookup"><span data-stu-id="2d063-109">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="2d063-110">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="2d063-110">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="2d063-111">Personalizada</span><span class="sxs-lookup"><span data-stu-id="2d063-111">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="2d063-112">justifyaction</span><span class="sxs-lookup"><span data-stu-id="2d063-112">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="2d063-113">metadataaction</span><span class="sxs-lookup"><span data-stu-id="2d063-113">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="2d063-114">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="2d063-114">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="2d063-115">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="2d063-115">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="2d063-116">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="2d063-116">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="2d063-117">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="2d063-117">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="2d063-118">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2d063-118">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="2d063-119">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2d063-119">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="2d063-120">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="2d063-120">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="2d063-121">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="2d063-121">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="2d063-122">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d063-122">Permissions</span></span>

<span data-ttu-id="2d063-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d063-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d063-125">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d063-125">Permission type</span></span>                        | <span data-ttu-id="2d063-126">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d063-126">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2d063-127">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d063-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d063-128">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="2d063-128">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="2d063-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d063-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d063-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d063-130">Not supported.</span></span>                              |
| <span data-ttu-id="2d063-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d063-131">Application</span></span>                            | <span data-ttu-id="2d063-132">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="2d063-132">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="2d063-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d063-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/informationprotection/policy/labels/evaluateApplication
POST /users/{id}/informationProtection/policy/labels/evaluateApplication
```

## <a name="request-headers"></a><span data-ttu-id="2d063-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d063-134">Request headers</span></span>

| <span data-ttu-id="2d063-135">Nome</span><span class="sxs-lookup"><span data-stu-id="2d063-135">Name</span></span>          | <span data-ttu-id="2d063-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d063-136">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="2d063-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d063-137">Authorization</span></span> | <span data-ttu-id="2d063-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d063-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2d063-140">Content-type</span><span class="sxs-lookup"><span data-stu-id="2d063-140">Content-type</span></span>  | <span data-ttu-id="2d063-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d063-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d063-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d063-143">Request body</span></span>

<span data-ttu-id="2d063-144">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d063-144">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d063-145">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2d063-145">Parameter</span></span>       | <span data-ttu-id="2d063-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d063-146">Type</span></span>                                               | <span data-ttu-id="2d063-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d063-147">Description</span></span>                                                                                                                                                                                                   |
| :-------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2d063-148">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2d063-148">contentInfo</span></span>     | [<span data-ttu-id="2d063-149">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2d063-149">contentInfo</span></span>](../resources/contentinfo.md)         | <span data-ttu-id="2d063-150">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="2d063-150">Provides details on the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="2d063-151">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="2d063-151">labelingOptions</span></span> | [<span data-ttu-id="2d063-152">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="2d063-152">labelingOptions</span></span>](../resources/labelingoptions.md) | <span data-ttu-id="2d063-153">Fornece detalhes sobre o estado desejado do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2d063-153">Provides details about the desired state of the content.</span></span>                                                                                                                                                      |

## <a name="response"></a><span data-ttu-id="2d063-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d063-154">Response</span></span>

<span data-ttu-id="2d063-155">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [informationProtectionAction](../resources/informationprotectionaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d063-155">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d063-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2d063-156">Examples</span></span>

<span data-ttu-id="2d063-157">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2d063-157">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2d063-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d063-158">Request</span></span>

<span data-ttu-id="2d063-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d063-159">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateApplication
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
  "labelingOptions": {
    "@odata.type": "#microsoft.graph.labelingOptions",
    "assignmentMethod@odata.type": "#microsoft.graph.assignmentMethod",
    "assignmentMethod": "standard",
    "labelId@odata.type": "#Guid",
    "labelId": "97309856-9c28-4ac6-9382-5f8bc20c457b",
    "downgradeJustification": null,
    "extendedProperties@odata.type": "#Collection(microsoft.graph.keyValuePair)",
    "extendedProperties": []
  }
}
```

### <a name="response"></a><span data-ttu-id="2d063-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d063-160">Response</span></span>

<span data-ttu-id="2d063-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2d063-161">The following is an example of the response.</span></span>

> <span data-ttu-id="2d063-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d063-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "@odata.type": "#microsoft.graph.protectByTemplateAction",
            "templateId": "31f2f3ba-1a56-48b7-ad90-0edc774ccfa2"
        },
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
            "metadataToAdd": [
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Enabled",
                    "value": "true"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_SetDate",
                    "value": "2019-10-03T21:40:02Z"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Method",
                    "value": "Standard"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Name",
                    "value": "Inspire Demo"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_SiteId",
                    "value": "cb46c030-1825-4e81-a295-151c039dbf02"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_ActionId",
                    "value": "987357d3-6512-46b5-b20e-000065400015"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_ContentBits",
                    "value": "8"
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
  "description": "informationProtectionLabel: evaluateApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
