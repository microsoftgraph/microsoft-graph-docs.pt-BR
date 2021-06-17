---
title: Criar cloudPcUserSetting
description: Crie um novo cloudPcUserSetting .
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: de9c9418796189b0f4d56f69672cd0c61f3da7b9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993634"
---
# <a name="create-cloudpcusersetting"></a><span data-ttu-id="227ee-103">Criar cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="227ee-103">Create cloudPcUserSetting</span></span>

<span data-ttu-id="227ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="227ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="227ee-105">Crie um novo [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="227ee-105">Create a new [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="227ee-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="227ee-106">Permissions</span></span>

<span data-ttu-id="227ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="227ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="227ee-109">Permission type</span></span>|<span data-ttu-id="227ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="227ee-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="227ee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="227ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="227ee-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227ee-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="227ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="227ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="227ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="227ee-114">Not supported.</span></span>|
|<span data-ttu-id="227ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="227ee-115">Application</span></span>|<span data-ttu-id="227ee-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="227ee-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="227ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="227ee-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings
```

## <a name="request-headers"></a><span data-ttu-id="227ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="227ee-118">Request headers</span></span>

| <span data-ttu-id="227ee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="227ee-119">Name</span></span>          | <span data-ttu-id="227ee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="227ee-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="227ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="227ee-121">Authorization</span></span> | <span data-ttu-id="227ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227ee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="227ee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="227ee-124">Content-Type</span></span>  | <span data-ttu-id="227ee-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="227ee-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="227ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="227ee-127">Request body</span></span>

<span data-ttu-id="227ee-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="227ee-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="227ee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcUserSetting](../resources/cloudpcusersetting.md).</span><span class="sxs-lookup"><span data-stu-id="227ee-129">The following table shows the properties that are required when you create the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="227ee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="227ee-130">Property</span></span>|<span data-ttu-id="227ee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="227ee-131">Type</span></span>|<span data-ttu-id="227ee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="227ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="227ee-133">displayName</span><span class="sxs-lookup"><span data-stu-id="227ee-133">displayName</span></span>|<span data-ttu-id="227ee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="227ee-134">String</span></span>|<span data-ttu-id="227ee-135">O nome da configuração como ele aparece na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="227ee-135">The setting name as it appears in the UI.</span></span> |
|<span data-ttu-id="227ee-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="227ee-136">localAdminEnabled</span></span>|<span data-ttu-id="227ee-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="227ee-137">Boolean</span></span>|<span data-ttu-id="227ee-138">Para ativar a opção de administrador local, altere essa configuração para `True` . </span><span class="sxs-lookup"><span data-stu-id="227ee-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="227ee-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="227ee-139">selfServiceEnabled</span></span>|<span data-ttu-id="227ee-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="227ee-140">Boolean</span></span>|<span data-ttu-id="227ee-141">Para ativar a opção self service, altere essa configuração para `True` . </span><span class="sxs-lookup"><span data-stu-id="227ee-141">To turn on the self service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="227ee-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="227ee-142">lastModifiedDateTime</span></span>|<span data-ttu-id="227ee-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="227ee-143">DateTimeOffset</span></span>|<span data-ttu-id="227ee-144">A última data e hora em que a configuração foi modificada.</span><span class="sxs-lookup"><span data-stu-id="227ee-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="227ee-145">O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="227ee-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="227ee-146">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="227ee-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |

## <a name="response"></a><span data-ttu-id="227ee-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="227ee-147">Response</span></span>

<span data-ttu-id="227ee-148">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto cloudPcUserSetting](../resources/cloudpcusersetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="227ee-148">If successful, this method returns a `201 Created` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="227ee-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="227ee-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="227ee-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="227ee-150">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="227ee-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="227ee-151">Response</span></span>
><span data-ttu-id="227ee-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="227ee-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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

