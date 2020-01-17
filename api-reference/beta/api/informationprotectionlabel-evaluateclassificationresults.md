---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: Avaliar qual rótulo aplicar com base nas informações de conteúdo existentes e em um resultado de classificação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f1012e7516ee635d9b44d1ae8a1277480aff6c8
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216670"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a><span data-ttu-id="22920-103">informationProtectionLabel: evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="22920-103">informationProtectionLabel: evaluateClassificationResults</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22920-104">Usando [os resultados da classificação](../resources/classificationresult.md), calcule o [rótulo de proteção de informações](../resources/informationprotectionlabel.md) que deve ser aplicado e retorne o conjunto de ações que devem ser executadas para rotular corretamente as informações.</span><span class="sxs-lookup"><span data-stu-id="22920-104">Using [classification results](../resources/classificationresult.md), compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="22920-105">Essa API é útil quando um rótulo deve ser definido automaticamente com base na classificação do conteúdo do arquivo, em vez de ser rotulado diretamente por um usuário ou serviço.</span><span class="sxs-lookup"><span data-stu-id="22920-105">This API is useful when a label should be set automatically based on classification of the file contents, rather than labeled directly by a user or service.</span></span> 

<span data-ttu-id="22920-106">Para avaliar com base nos resultados da classificação, forneça [contentInfo](../resources/contentinfo.md), que inclui [pares de chave/valor](../resources/keyvaluepair.md)de metadados de conteúdo existentes e [resultados da classificação](../resources/classificationresult.md).</span><span class="sxs-lookup"><span data-stu-id="22920-106">To evaluate based on classification results, provide [contentInfo](../resources/contentinfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [classification results](../resources/classificationresult.md).</span></span> <span data-ttu-id="22920-107">A API retorna um [informationProtectionAction](../resources/informationprotectionaction.md) que contém um ou mais dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="22920-107">The API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains one of more of the following:</span></span> 

* [<span data-ttu-id="22920-108">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="22920-108">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="22920-109">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="22920-109">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="22920-110">addwatermarkaction</span><span class="sxs-lookup"><span data-stu-id="22920-110">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="22920-111">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="22920-111">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="22920-112">Personalizada</span><span class="sxs-lookup"><span data-stu-id="22920-112">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="22920-113">justifyaction</span><span class="sxs-lookup"><span data-stu-id="22920-113">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="22920-114">metadataaction</span><span class="sxs-lookup"><span data-stu-id="22920-114">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="22920-115">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="22920-115">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="22920-116">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="22920-116">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="22920-117">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="22920-117">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="22920-118">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="22920-118">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="22920-119">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="22920-119">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="22920-120">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="22920-120">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="22920-121">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="22920-121">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="22920-122">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="22920-122">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="22920-123">Permissões</span><span class="sxs-lookup"><span data-stu-id="22920-123">Permissions</span></span>

<span data-ttu-id="22920-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22920-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22920-126">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22920-126">Permission type</span></span>                        | <span data-ttu-id="22920-127">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22920-127">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="22920-128">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22920-128">Delegated (work or school account)</span></span>     | <span data-ttu-id="22920-129">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="22920-129">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="22920-130">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22920-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22920-131">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22920-131">Not supported.</span></span>                              |
| <span data-ttu-id="22920-132">Application</span><span class="sxs-lookup"><span data-stu-id="22920-132">Application</span></span>                            | <span data-ttu-id="22920-133">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="22920-133">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="22920-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22920-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a><span data-ttu-id="22920-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22920-135">Request headers</span></span>

| <span data-ttu-id="22920-136">Nome</span><span class="sxs-lookup"><span data-stu-id="22920-136">Name</span></span>          | <span data-ttu-id="22920-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="22920-137">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="22920-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="22920-138">Authorization</span></span> | <span data-ttu-id="22920-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22920-p104">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="22920-141">Content-type</span><span class="sxs-lookup"><span data-stu-id="22920-141">Content-type</span></span>  | <span data-ttu-id="22920-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22920-p105">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="22920-144">Agente de usuário</span><span class="sxs-lookup"><span data-stu-id="22920-144">User-Agent</span></span>    | <span data-ttu-id="22920-145">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="22920-145">Describes the name and version of the calling application.</span></span> <span data-ttu-id="22920-146">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="22920-146">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="22920-147">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="22920-147">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="22920-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="22920-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22920-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22920-149">Request body</span></span>

<span data-ttu-id="22920-150">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22920-150">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22920-151">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="22920-151">Parameter</span></span>             | <span data-ttu-id="22920-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="22920-152">Type</span></span>                                                                    | <span data-ttu-id="22920-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="22920-153">Description</span></span>                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="22920-154">contentInfo</span><span class="sxs-lookup"><span data-stu-id="22920-154">contentInfo</span></span>           | [<span data-ttu-id="22920-155">contentInfo</span><span class="sxs-lookup"><span data-stu-id="22920-155">contentInfo</span></span>](../resources/contentInfo.md)                              | <span data-ttu-id="22920-156">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="22920-156">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span>                                                                                                                                                   |
| <span data-ttu-id="22920-157">classificationResults</span><span class="sxs-lookup"><span data-stu-id="22920-157">classificationResults</span></span> | <span data-ttu-id="22920-158">coleção [classificationResult](../resources/classificationresult.md)</span><span class="sxs-lookup"><span data-stu-id="22920-158">[classificationResult](../resources/classificationresult.md) collection</span></span> | <span data-ttu-id="22920-159">Contém o conjunto de resultados de classificação retornado pelo ponto de extremidade de classificação de dados.</span><span class="sxs-lookup"><span data-stu-id="22920-159">Contains the set of classification results returned by the data classification endpoint.</span></span> <span data-ttu-id="22920-160">As informações de Classificaiton são usadas para determinar o rótulo apropriado com base na configuração de rótulo de política de proteção de informações da Microsoft no centro de segurança e conformidade do Office 365.</span><span class="sxs-lookup"><span data-stu-id="22920-160">Classificaiton information is used to determine the appropriate label based on the Microsoft Information Protection policy label configuration in Office 365 Security and Compliance Center.</span></span> |

## <a name="response"></a><span data-ttu-id="22920-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="22920-161">Response</span></span>

<span data-ttu-id="22920-162">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto da coleção [informationProtectionAction](../resources/informationprotectionaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22920-162">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22920-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22920-163">Examples</span></span>

<span data-ttu-id="22920-164">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="22920-164">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="22920-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22920-165">Request</span></span>

<span data-ttu-id="22920-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22920-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22920-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="22920-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateClassificationResults
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="22920-168">C#</span><span class="sxs-lookup"><span data-stu-id="22920-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22920-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22920-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22920-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22920-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22920-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="22920-171">Response</span></span>

<span data-ttu-id="22920-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22920-172">The following is an example of the response.</span></span>

> <span data-ttu-id="22920-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22920-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
