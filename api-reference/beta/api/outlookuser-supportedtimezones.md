---
title: 'outlookUser: supportedTimeZones'
description: Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f54457169b4f4f214488727fa94b7402b0f33724
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963558"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="58a55-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="58a55-103">outlookUser: supportedTimeZones</span></span>

> <span data-ttu-id="58a55-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="58a55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58a55-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58a55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58a55-106">Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="58a55-106">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="58a55-107">É possível especificar explicitamente que os fusos horário sejam retornados no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="58a55-107">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="58a55-108">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="58a55-108">The Windows format is the default.</span></span>

<span data-ttu-id="58a55-109">Ao configurar um cliente do Outlook, o usuário seleciona o fuso horário na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="58a55-109">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="58a55-110">Posteriormente, é possível obter o fuso horário de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="58a55-110">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="58a55-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="58a55-111">Permissions</span></span>
<span data-ttu-id="58a55-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58a55-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a55-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58a55-114">Permission type</span></span>      | <span data-ttu-id="58a55-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58a55-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58a55-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58a55-116">Delegated (work or school account)</span></span> | <span data-ttu-id="58a55-117">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="58a55-117">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="58a55-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58a55-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58a55-119">User.Read</span><span class="sxs-lookup"><span data-stu-id="58a55-119">User.Read</span></span>    |
|<span data-ttu-id="58a55-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58a55-120">Application</span></span> | <span data-ttu-id="58a55-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a55-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58a55-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58a55-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="58a55-123">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="58a55-123">Function parameters</span></span>
| <span data-ttu-id="58a55-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58a55-124">Parameter</span></span>      | <span data-ttu-id="58a55-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="58a55-125">Type</span></span>    | <span data-ttu-id="58a55-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="58a55-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58a55-127">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="58a55-127">TimeZoneStandard</span></span>  | <span data-ttu-id="58a55-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58a55-128">String</span></span>  | <span data-ttu-id="58a55-129">Um formato de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="58a55-129">A time zone format.</span></span> <span data-ttu-id="58a55-130">Os valores com suporte são: `Windows` e `Iana`.</span><span class="sxs-lookup"><span data-stu-id="58a55-130">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="58a55-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="58a55-131">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="58a55-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58a55-132">Request headers</span></span>
| <span data-ttu-id="58a55-133">Nome</span><span class="sxs-lookup"><span data-stu-id="58a55-133">Name</span></span>       | <span data-ttu-id="58a55-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="58a55-134">Type</span></span> | <span data-ttu-id="58a55-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="58a55-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="58a55-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="58a55-136">Authorization</span></span>  | <span data-ttu-id="58a55-137">string</span><span class="sxs-lookup"><span data-stu-id="58a55-137">string</span></span>  | <span data-ttu-id="58a55-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58a55-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58a55-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58a55-140">Request body</span></span>
<span data-ttu-id="58a55-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58a55-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58a55-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a55-142">Response</span></span>
<span data-ttu-id="58a55-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [timeZoneInformation](../resources/timezoneinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a55-143">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a55-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58a55-144">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="58a55-145">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="58a55-145">Request 1</span></span>
<span data-ttu-id="58a55-146">O exemplo a seguir não especifica o parâmetro `timeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato do Windows.</span><span class="sxs-lookup"><span data-stu-id="58a55-146">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="58a55-147">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="58a55-147">Response 1</span></span>
<span data-ttu-id="58a55-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a55-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```

##### <a name="request-2"></a><span data-ttu-id="58a55-149">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="58a55-149">Request 2</span></span>
<span data-ttu-id="58a55-150">O exemplo a seguir especifica `Iana` para o parâmetro `TimeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato da IANA.</span><span class="sxs-lookup"><span data-stu-id="58a55-150">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="58a55-151">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="58a55-151">Response 2</span></span>
<span data-ttu-id="58a55-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a55-152">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
