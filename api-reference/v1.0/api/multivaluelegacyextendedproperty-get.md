---
title: Obter multiValueLegacyExtendedProperty
description: Expanda '.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8b014ea576f08b19f10d8943350dfc25983cf1d5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812376"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="015ac-103">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="015ac-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="015ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="015ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="015ac-105">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="015ac-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="015ac-106">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada.</span><span class="sxs-lookup"><span data-stu-id="015ac-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="015ac-107">Atualmente, esta é a única maneira de obter o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="015ac-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="015ac-108">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="015ac-108">The following user resources are supported:</span></span>

- [<span data-ttu-id="015ac-109">calendar</span><span class="sxs-lookup"><span data-stu-id="015ac-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="015ac-110">contact</span><span class="sxs-lookup"><span data-stu-id="015ac-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="015ac-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="015ac-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="015ac-112">event</span><span class="sxs-lookup"><span data-stu-id="015ac-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="015ac-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="015ac-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="015ac-114">message</span><span class="sxs-lookup"><span data-stu-id="015ac-114">message</span></span>](../resources/message.md)

<span data-ttu-id="015ac-115">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="015ac-115">As well as the following group resources:</span></span>

- <span data-ttu-id="015ac-116">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="015ac-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="015ac-117">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="015ac-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="015ac-118">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="015ac-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="015ac-119">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="015ac-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="015ac-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="015ac-120">Permissions</span></span>
<span data-ttu-id="015ac-121">Dependendo do recurso para o qual você está obtendo a propriedade estendida e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="015ac-121">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="015ac-122">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="015ac-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="015ac-123">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="015ac-123">Supported resource</span></span> | <span data-ttu-id="015ac-124">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="015ac-124">Delegated (work or school account)</span></span> | <span data-ttu-id="015ac-125">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="015ac-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="015ac-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="015ac-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="015ac-127">calendar</span><span class="sxs-lookup"><span data-stu-id="015ac-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="015ac-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-128">Calendars.Read</span></span> | <span data-ttu-id="015ac-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-129">Calendars.Read</span></span> | <span data-ttu-id="015ac-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-130">Calendars.Read</span></span> |
| [<span data-ttu-id="015ac-131">contato</span><span class="sxs-lookup"><span data-stu-id="015ac-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="015ac-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-132">Contacts.Read</span></span> | <span data-ttu-id="015ac-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-133">Contacts.Read</span></span> | <span data-ttu-id="015ac-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-134">Contacts.Read</span></span> |
| [<span data-ttu-id="015ac-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="015ac-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="015ac-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-136">Contacts.Read</span></span> | <span data-ttu-id="015ac-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-137">Contacts.Read</span></span> | <span data-ttu-id="015ac-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-138">Contacts.Read</span></span> |
| [<span data-ttu-id="015ac-139">evento</span><span class="sxs-lookup"><span data-stu-id="015ac-139">event</span></span>](../resources/event.md) | <span data-ttu-id="015ac-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-140">Calendars.Read</span></span> | <span data-ttu-id="015ac-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-141">Calendars.Read</span></span> |  <span data-ttu-id="015ac-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-142">Calendars.Read</span></span>|
| <span data-ttu-id="015ac-143">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="015ac-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="015ac-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="015ac-144">Group.Read.All</span></span> | <span data-ttu-id="015ac-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="015ac-145">Not supported</span></span> | <span data-ttu-id="015ac-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="015ac-146">Not supported</span></span> |
| <span data-ttu-id="015ac-147">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="015ac-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="015ac-148">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="015ac-148">Group.Read.All</span></span> | <span data-ttu-id="015ac-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="015ac-149">Not supported</span></span> | <span data-ttu-id="015ac-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="015ac-150">Not supported</span></span> |
| <span data-ttu-id="015ac-151">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="015ac-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="015ac-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="015ac-152">Group.Read.All</span></span> | <span data-ttu-id="015ac-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="015ac-153">Not supported</span></span> | <span data-ttu-id="015ac-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="015ac-154">Group.Read.All</span></span> |
| [<span data-ttu-id="015ac-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="015ac-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="015ac-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-156">Mail.Read</span></span> | <span data-ttu-id="015ac-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-157">Mail.Read</span></span> | <span data-ttu-id="015ac-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-158">Mail.Read</span></span> |
| [<span data-ttu-id="015ac-159">message</span><span class="sxs-lookup"><span data-stu-id="015ac-159">message</span></span>](../resources/message.md) | <span data-ttu-id="015ac-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-160">Mail.Read</span></span> | <span data-ttu-id="015ac-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-161">Mail.Read</span></span> | <span data-ttu-id="015ac-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="015ac-162">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="015ac-163">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="015ac-163">HTTP request</span></span>

<span data-ttu-id="015ac-p103">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="015ac-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="015ac-166">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="015ac-166">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="015ac-167">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="015ac-167">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="015ac-168">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="015ac-168">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="015ac-169">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="015ac-169">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="015ac-170">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="015ac-170">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="015ac-171">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="015ac-171">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="015ac-172">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="015ac-172">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="015ac-173">Acesse uma instância de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="015ac-173">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="015ac-174">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="015ac-174">Path parameters</span></span>
|<span data-ttu-id="015ac-175">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="015ac-175">Parameter</span></span>|<span data-ttu-id="015ac-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="015ac-176">Type</span></span>|<span data-ttu-id="015ac-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="015ac-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="015ac-178">id_value</span><span class="sxs-lookup"><span data-stu-id="015ac-178">id_value</span></span>|<span data-ttu-id="015ac-179">String</span><span class="sxs-lookup"><span data-stu-id="015ac-179">String</span></span>|<span data-ttu-id="015ac-p104">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="015ac-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="015ac-184">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="015ac-184">Request headers</span></span>
| <span data-ttu-id="015ac-185">Nome</span><span class="sxs-lookup"><span data-stu-id="015ac-185">Name</span></span>      |<span data-ttu-id="015ac-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="015ac-186">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="015ac-187">Autorização</span><span class="sxs-lookup"><span data-stu-id="015ac-187">Authorization</span></span>  | <span data-ttu-id="015ac-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="015ac-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="015ac-190">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="015ac-190">Request body</span></span>
<span data-ttu-id="015ac-191">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="015ac-191">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="015ac-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="015ac-192">Response</span></span>

<span data-ttu-id="015ac-193">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="015ac-193">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="015ac-194">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="015ac-194">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="015ac-195">Exemplo</span><span class="sxs-lookup"><span data-stu-id="015ac-195">Example</span></span>
##### <a name="request"></a><span data-ttu-id="015ac-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="015ac-196">Request</span></span>
<span data-ttu-id="015ac-p106">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="015ac-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="015ac-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="015ac-199">Response</span></span>

<span data-ttu-id="015ac-200">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="015ac-200">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="015ac-p107">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="015ac-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
