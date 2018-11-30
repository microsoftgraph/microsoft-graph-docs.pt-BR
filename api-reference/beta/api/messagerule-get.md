---
title: Obter regra
description: Obtenha as propriedades e as relações de um objeto messageRule.
ms.openlocfilehash: 0151a83f54c67e6daf5c78766f6d4a532108bfda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040441"
---
# <a name="get-rule"></a><span data-ttu-id="3abee-103">Obter regra</span><span class="sxs-lookup"><span data-stu-id="3abee-103">Get rule</span></span>

> <span data-ttu-id="3abee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3abee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3abee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3abee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3abee-106">Obtenha as propriedades e as relações de um objeto [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="3abee-106">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="3abee-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3abee-107">Permissions</span></span>
<span data-ttu-id="3abee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3abee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3abee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3abee-110">Permission type</span></span>      | <span data-ttu-id="3abee-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3abee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3abee-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3abee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3abee-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="3abee-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="3abee-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3abee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3abee-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="3abee-115">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="3abee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3abee-116">Application</span></span> | <span data-ttu-id="3abee-117">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="3abee-117">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3abee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3abee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3abee-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3abee-119">Optional query parameters</span></span>
<span data-ttu-id="3abee-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3abee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3abee-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3abee-121">Request headers</span></span>
| <span data-ttu-id="3abee-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3abee-122">Name</span></span>      |<span data-ttu-id="3abee-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3abee-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3abee-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3abee-124">Authorization</span></span>  | <span data-ttu-id="3abee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3abee-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3abee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3abee-127">Request body</span></span>
<span data-ttu-id="3abee-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3abee-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3abee-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3abee-129">Response</span></span>
<span data-ttu-id="3abee-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3abee-130">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3abee-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3abee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3abee-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3abee-132">Request</span></span>
<span data-ttu-id="3abee-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3abee-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
##### <a name="response"></a><span data-ttu-id="3abee-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3abee-134">Response</span></span>
<span data-ttu-id="3abee-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3abee-135">Here is an example of the response.</span></span> <span data-ttu-id="3abee-136">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="3abee-136">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="3abee-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3abee-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->