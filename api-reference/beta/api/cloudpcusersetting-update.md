---
title: Atualizar cloudPcUserSetting
description: Atualize as propriedades de um objeto cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 2ea5b8f7084f2be8f4fd5d79345a69ee656f1fbb
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993632"
---
# <a name="update-cloudpcusersetting"></a><span data-ttu-id="ba114-103">Atualizar cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="ba114-103">Update cloudPcUserSetting</span></span>

<span data-ttu-id="ba114-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba114-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba114-105">Atualize as propriedades de [um objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba114-105">Update the properties of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ba114-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ba114-106">Permissions</span></span>

<span data-ttu-id="ba114-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba114-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba114-109">Permission type</span></span>|<span data-ttu-id="ba114-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba114-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba114-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba114-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba114-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba114-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ba114-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba114-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba114-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba114-114">Not supported.</span></span>|
|<span data-ttu-id="ba114-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba114-115">Application</span></span>|<span data-ttu-id="ba114-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba114-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba114-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba114-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba114-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba114-118">Request headers</span></span>

| <span data-ttu-id="ba114-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ba114-119">Name</span></span>          | <span data-ttu-id="ba114-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba114-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="ba114-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba114-121">Authorization</span></span> | <span data-ttu-id="ba114-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba114-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba114-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba114-124">Content-Type</span></span>  | <span data-ttu-id="ba114-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba114-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba114-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba114-127">Request body</span></span>

<span data-ttu-id="ba114-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba114-128">In the request body, supply a JSON representation of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

<span data-ttu-id="ba114-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o cloudPcUserSetting](../resources/cloudpcusersetting.md).</span><span class="sxs-lookup"><span data-stu-id="ba114-129">The following table shows the properties that are required when you update the [cloudPcUserSetting](../resources/cloudpcusersetting.md).</span></span>

|<span data-ttu-id="ba114-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba114-130">Property</span></span>|<span data-ttu-id="ba114-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba114-131">Type</span></span>|<span data-ttu-id="ba114-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba114-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba114-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ba114-133">displayName</span></span>|<span data-ttu-id="ba114-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba114-134">String</span></span>|<span data-ttu-id="ba114-135">O nome da configuração exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba114-135">The setting name displayed in the user interface.</span></span>|
|<span data-ttu-id="ba114-136">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="ba114-136">localAdminEnabled</span></span>|<span data-ttu-id="ba114-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba114-137">Boolean</span></span>|<span data-ttu-id="ba114-138">Para ativar a opção de administrador local, altere essa configuração para `True` . </span><span class="sxs-lookup"><span data-stu-id="ba114-138">To turn on the local admin option, change this setting to `True`. </span></span> |
|<span data-ttu-id="ba114-139">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="ba114-139">selfServiceEnabled</span></span>|<span data-ttu-id="ba114-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba114-140">Boolean</span></span>|<span data-ttu-id="ba114-141">Para ativar a opção self-service, altere essa configuração para `True` . </span><span class="sxs-lookup"><span data-stu-id="ba114-141">To turn on the self-service option, change this setting to `True`. </span></span>|
|<span data-ttu-id="ba114-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba114-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ba114-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba114-143">DateTimeOffset</span></span>|<span data-ttu-id="ba114-144">A última data e hora em que a configuração foi modificada.</span><span class="sxs-lookup"><span data-stu-id="ba114-144">The last date and time the setting was modified.</span></span> <span data-ttu-id="ba114-145">O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ba114-145">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ba114-146">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="ba114-146">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |



## <a name="response"></a><span data-ttu-id="ba114-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba114-147">Response</span></span>

<span data-ttu-id="ba114-148">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcUserSetting](../resources/cloudpcusersetting.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba114-148">If successful, this method returns a `200 OK` response code and an updated [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba114-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba114-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba114-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba114-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_cloudpcusersetting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff
Content-Type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "displayName": "Example",
  "selfServiceEnabled": true,
  "localAdminEnabled": false
}
```


### <a name="response"></a><span data-ttu-id="ba114-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba114-151">Response</span></span>
><span data-ttu-id="ba114-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ba114-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
