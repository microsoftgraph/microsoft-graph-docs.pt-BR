---
title: Criar deviceManagementIntent
description: Criar um novo objeto deviceManagementIntent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea9dd1754d3482d8fc0eedcba49d5674e5f73ea5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471558"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="c7a9f-103">Criar deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="c7a9f-103">Create deviceManagementIntent</span></span>

<span data-ttu-id="c7a9f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7a9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7a9f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7a9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7a9f-107">Criar um novo objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="c7a9f-107">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7a9f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c7a9f-108">Prerequisites</span></span>
<span data-ttu-id="c7a9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7a9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7a9f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7a9f-111">Permission type</span></span>|<span data-ttu-id="c7a9f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c7a9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7a9f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7a9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7a9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7a9f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7a9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7a9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-116">Not supported.</span></span>|
|<span data-ttu-id="c7a9f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7a9f-117">Application</span></span>|<span data-ttu-id="c7a9f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7a9f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7a9f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7a9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="c7a9f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a9f-120">Request headers</span></span>
|<span data-ttu-id="c7a9f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7a9f-121">Header</span></span>|<span data-ttu-id="c7a9f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7a9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7a9f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7a9f-123">Authorization</span></span>|<span data-ttu-id="c7a9f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7a9f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c7a9f-125">Accept</span></span>|<span data-ttu-id="c7a9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7a9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7a9f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a9f-127">Request body</span></span>
<span data-ttu-id="c7a9f-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-128">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="c7a9f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-129">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="c7a9f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7a9f-130">Property</span></span>|<span data-ttu-id="c7a9f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a9f-131">Type</span></span>|<span data-ttu-id="c7a9f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7a9f-133">id</span><span class="sxs-lookup"><span data-stu-id="c7a9f-133">id</span></span>|<span data-ttu-id="c7a9f-134">String</span><span class="sxs-lookup"><span data-stu-id="c7a9f-134">String</span></span>|<span data-ttu-id="c7a9f-135">A ID de intenção</span><span class="sxs-lookup"><span data-stu-id="c7a9f-135">The intent ID</span></span>|
|<span data-ttu-id="c7a9f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c7a9f-136">displayName</span></span>|<span data-ttu-id="c7a9f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7a9f-137">String</span></span>|<span data-ttu-id="c7a9f-138">O nome de exibição fornecido pelo usuário</span><span class="sxs-lookup"><span data-stu-id="c7a9f-138">The user given display name</span></span>|
|<span data-ttu-id="c7a9f-139">description</span><span class="sxs-lookup"><span data-stu-id="c7a9f-139">description</span></span>|<span data-ttu-id="c7a9f-140">String</span><span class="sxs-lookup"><span data-stu-id="c7a9f-140">String</span></span>|<span data-ttu-id="c7a9f-141">Descrição fornecida pelo usuário</span><span class="sxs-lookup"><span data-stu-id="c7a9f-141">The user given description</span></span>|
|<span data-ttu-id="c7a9f-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c7a9f-142">isAssigned</span></span>|<span data-ttu-id="c7a9f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7a9f-143">Boolean</span></span>|<span data-ttu-id="c7a9f-144">Significa se a intenção é atribuída ou não aos usuários</span><span class="sxs-lookup"><span data-stu-id="c7a9f-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="c7a9f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7a9f-145">lastModifiedDateTime</span></span>|<span data-ttu-id="c7a9f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7a9f-146">DateTimeOffset</span></span>|<span data-ttu-id="c7a9f-147">Quando a intenção foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="c7a9f-147">When the intent was last modified</span></span>|
|<span data-ttu-id="c7a9f-148">templateId</span><span class="sxs-lookup"><span data-stu-id="c7a9f-148">templateId</span></span>|<span data-ttu-id="c7a9f-149">String</span><span class="sxs-lookup"><span data-stu-id="c7a9f-149">String</span></span>|<span data-ttu-id="c7a9f-150">A ID do modelo de que esta intenção foi criada (se houver)</span><span class="sxs-lookup"><span data-stu-id="c7a9f-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="c7a9f-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7a9f-151">roleScopeTagIds</span></span>|<span data-ttu-id="c7a9f-152">String collection</span><span class="sxs-lookup"><span data-stu-id="c7a9f-152">String collection</span></span>|<span data-ttu-id="c7a9f-153">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c7a9f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a9f-154">Response</span></span>
<span data-ttu-id="c7a9f-155">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7a9f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7a9f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7a9f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7a9f-157">Request</span></span>
<span data-ttu-id="c7a9f-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c7a9f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7a9f-159">Response</span></span>
<span data-ttu-id="c7a9f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7a9f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





