---
title: Criar cloudPcUserSetting
description: Crie um novo cloudPcUserSetting .
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3edffeab1a7eaf4cac05200093d0f7a49d840614
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208495"
---
# <a name="create-cloudpcusersetting"></a><span data-ttu-id="00b64-103">Criar cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="00b64-103">Create cloudPcUserSetting</span></span>

<span data-ttu-id="00b64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00b64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00b64-105">Crie um novo [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="00b64-105">Create a new [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="00b64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00b64-106">Permissions</span></span>

<span data-ttu-id="00b64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00b64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00b64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00b64-109">Permission type</span></span>|<span data-ttu-id="00b64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00b64-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00b64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00b64-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00b64-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b64-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="00b64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00b64-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00b64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00b64-114">Not supported.</span></span>|
|<span data-ttu-id="00b64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00b64-115">Application</span></span>|<span data-ttu-id="00b64-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00b64-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00b64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00b64-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings
```

## <a name="request-headers"></a><span data-ttu-id="00b64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00b64-118">Request headers</span></span>

| <span data-ttu-id="00b64-119">Nome</span><span class="sxs-lookup"><span data-stu-id="00b64-119">Name</span></span>          | <span data-ttu-id="00b64-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="00b64-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="00b64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="00b64-121">Authorization</span></span> | <span data-ttu-id="00b64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00b64-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00b64-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00b64-124">Content-Type</span></span>  | <span data-ttu-id="00b64-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00b64-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00b64-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00b64-127">Request body</span></span>

<span data-ttu-id="00b64-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="00b64-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="00b64-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcUserSetting](../resources/cloudpcusersetting.md).</span><span class="sxs-lookup"><span data-stu-id="00b64-129">The following table shows the properties that are required when you create the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="00b64-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00b64-130">Property</span></span>|<span data-ttu-id="00b64-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00b64-131">Type</span></span>|<span data-ttu-id="00b64-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00b64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00b64-133">displayName</span><span class="sxs-lookup"><span data-stu-id="00b64-133">displayName</span></span>|<span data-ttu-id="00b64-134">String</span><span class="sxs-lookup"><span data-stu-id="00b64-134">String</span></span>|<span data-ttu-id="00b64-135">O nome da configuração como ele aparece na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="00b64-135">The setting name as it appears in the UI.</span></span> |
|<span data-ttu-id="00b64-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="00b64-136">localAdminEnabled</span></span>|<span data-ttu-id="00b64-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="00b64-137">Boolean</span></span>|<span data-ttu-id="00b64-138">Para ativar a opção de administrador local, altere essa configuração para `True` . </span><span class="sxs-lookup"><span data-stu-id="00b64-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="00b64-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="00b64-139">selfServiceEnabled</span></span>|<span data-ttu-id="00b64-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="00b64-140">Boolean</span></span>|<span data-ttu-id="00b64-141">Para ativar a opção self service, altere essa configuração para `True` . </span><span class="sxs-lookup"><span data-stu-id="00b64-141">To turn on the self service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="00b64-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00b64-142">lastModifiedDateTime</span></span>|<span data-ttu-id="00b64-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00b64-143">DateTimeOffset</span></span>|<span data-ttu-id="00b64-144">A última data e hora em que a configuração foi modificada.</span><span class="sxs-lookup"><span data-stu-id="00b64-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="00b64-145">O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="00b64-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00b64-146">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="00b64-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |

## <a name="response"></a><span data-ttu-id="00b64-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="00b64-147">Response</span></span>

<span data-ttu-id="00b64-148">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cloudPcUserSetting](../resources/cloudpcusersetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00b64-148">If successful, this method returns a `201 Created` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00b64-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00b64-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00b64-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00b64-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="00b64-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="00b64-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcusersetting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="00b64-152">C#</span><span class="sxs-lookup"><span data-stu-id="00b64-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcusersetting-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00b64-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00b64-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcusersetting-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00b64-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00b64-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcusersetting-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00b64-155">Java</span><span class="sxs-lookup"><span data-stu-id="00b64-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcusersetting-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="00b64-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="00b64-156">Response</span></span>
><span data-ttu-id="00b64-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="00b64-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "556092f8-92f8-5560-f892-6055f8926055",
  "displayName": "Example",
  "selfServiceEnabled": false,
  "localAdminEnabled": true,
  "lastModifiedDateTime": "2021-02-01T10:29:57Z"  
}
```

