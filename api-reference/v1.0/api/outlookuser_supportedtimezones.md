# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="3c4ae-101">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="3c4ae-101">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="3c4ae-102">Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-102">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="3c4ae-103">É possível especificar explicitamente que os fusos horário sejam retornados no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="3c4ae-103">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="3c4ae-104">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-104">The Windows format is the default.</span></span>

<span data-ttu-id="3c4ae-105">Ao configurar um cliente do Outlook, o usuário seleciona o fuso horário na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-105">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="3c4ae-106">Posteriormente, é possível obter o fuso horário de sua preferência [acessando as configurações da caixa de correio do usuário](user_get_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3c4ae-106">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="3c4ae-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c4ae-107">Permissions</span></span>
<span data-ttu-id="3c4ae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c4ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c4ae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c4ae-110">Permission type</span></span>      | <span data-ttu-id="3c4ae-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c4ae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c4ae-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c4ae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c4ae-113">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="3c4ae-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="3c4ae-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c4ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c4ae-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="3c4ae-115">User.Read</span></span>    |
|<span data-ttu-id="3c4ae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c4ae-116">Application</span></span> | <span data-ttu-id="3c4ae-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c4ae-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c4ae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c4ae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="3c4ae-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="3c4ae-119">Function parameters</span></span>
| <span data-ttu-id="3c4ae-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3c4ae-120">Parameter</span></span>       | <span data-ttu-id="3c4ae-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c4ae-121">Type</span></span> | <span data-ttu-id="3c4ae-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c4ae-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c4ae-123">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="3c4ae-123">TimeZoneStandard</span></span>  | <span data-ttu-id="3c4ae-124">timeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="3c4ae-124">timeZoneStandard</span></span>  | <span data-ttu-id="3c4ae-125">Um formato de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-125">A time zone format.</span></span> <span data-ttu-id="3c4ae-126">Os valores com suporte são: `Windows` e `Iana`.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-126">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="3c4ae-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-127">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3c4ae-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c4ae-128">Request headers</span></span>
| <span data-ttu-id="3c4ae-129">Nome</span><span class="sxs-lookup"><span data-stu-id="3c4ae-129">Name</span></span>       | <span data-ttu-id="3c4ae-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c4ae-130">Type</span></span> | <span data-ttu-id="3c4ae-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c4ae-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c4ae-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c4ae-132">Authorization</span></span>  | <span data-ttu-id="3c4ae-133">string</span><span class="sxs-lookup"><span data-stu-id="3c4ae-133">string</span></span>  | <span data-ttu-id="3c4ae-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c4ae-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c4ae-136">Request body</span></span>
<span data-ttu-id="3c4ae-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c4ae-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c4ae-138">Response</span></span>
<span data-ttu-id="3c4ae-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [timeZoneInformation](../resources/timezoneinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-139">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c4ae-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3c4ae-140">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="3c4ae-141">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="3c4ae-141">Request 1</span></span>
<span data-ttu-id="3c4ae-142">O exemplo a seguir não especifica o parâmetro `timeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato do Windows.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-142">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="3c4ae-143">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="3c4ae-143">Response 1</span></span>
<span data-ttu-id="3c4ae-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-144">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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

##### <a name="request-2"></a><span data-ttu-id="3c4ae-145">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="3c4ae-145">Request 2</span></span>
<span data-ttu-id="3c4ae-146">O exemplo a seguir especifica `Iana` para o parâmetro `TimeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato da IANA.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-146">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="3c4ae-147">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="3c4ae-147">Response 2</span></span>
<span data-ttu-id="3c4ae-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-148">Here is an example of the response.</span></span> 

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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