---
title: Criar deviceManagementIntent
description: Criar um novo objeto deviceManagementIntent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 937fe05d91c59e6162bc1140d9a664fdc40f4f25
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729574"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="71907-103">Criar deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="71907-103">Create deviceManagementIntent</span></span>

> <span data-ttu-id="71907-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71907-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71907-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71907-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71907-106">Criar um novo objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="71907-106">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71907-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71907-107">Prerequisites</span></span>
<span data-ttu-id="71907-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71907-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71907-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71907-110">Permission type</span></span>|<span data-ttu-id="71907-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71907-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71907-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71907-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71907-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71907-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71907-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71907-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71907-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71907-115">Not supported.</span></span>|
|<span data-ttu-id="71907-116">Application</span><span class="sxs-lookup"><span data-stu-id="71907-116">Application</span></span>|<span data-ttu-id="71907-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71907-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71907-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71907-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="71907-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71907-119">Request headers</span></span>
|<span data-ttu-id="71907-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71907-120">Header</span></span>|<span data-ttu-id="71907-121">Valor</span><span class="sxs-lookup"><span data-stu-id="71907-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71907-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71907-122">Authorization</span></span>|<span data-ttu-id="71907-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71907-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71907-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71907-124">Accept</span></span>|<span data-ttu-id="71907-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71907-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71907-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71907-126">Request body</span></span>
<span data-ttu-id="71907-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="71907-127">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="71907-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="71907-128">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="71907-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71907-129">Property</span></span>|<span data-ttu-id="71907-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="71907-130">Type</span></span>|<span data-ttu-id="71907-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="71907-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71907-132">id</span><span class="sxs-lookup"><span data-stu-id="71907-132">id</span></span>|<span data-ttu-id="71907-133">String</span><span class="sxs-lookup"><span data-stu-id="71907-133">String</span></span>|<span data-ttu-id="71907-134">A ID de intenção</span><span class="sxs-lookup"><span data-stu-id="71907-134">The intent ID</span></span>|
|<span data-ttu-id="71907-135">displayName</span><span class="sxs-lookup"><span data-stu-id="71907-135">displayName</span></span>|<span data-ttu-id="71907-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71907-136">String</span></span>|<span data-ttu-id="71907-137">O nome de exibição fornecido pelo usuário</span><span class="sxs-lookup"><span data-stu-id="71907-137">The user given display name</span></span>|
|<span data-ttu-id="71907-138">description</span><span class="sxs-lookup"><span data-stu-id="71907-138">description</span></span>|<span data-ttu-id="71907-139">String</span><span class="sxs-lookup"><span data-stu-id="71907-139">String</span></span>|<span data-ttu-id="71907-140">Descrição fornecida pelo usuário</span><span class="sxs-lookup"><span data-stu-id="71907-140">The user given description</span></span>|
|<span data-ttu-id="71907-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="71907-141">isAssigned</span></span>|<span data-ttu-id="71907-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="71907-142">Boolean</span></span>|<span data-ttu-id="71907-143">Significa se a intenção é atribuída ou não aos usuários</span><span class="sxs-lookup"><span data-stu-id="71907-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="71907-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71907-144">lastModifiedDateTime</span></span>|<span data-ttu-id="71907-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71907-145">DateTimeOffset</span></span>|<span data-ttu-id="71907-146">Quando a intenção foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="71907-146">When the intent was last modified</span></span>|
|<span data-ttu-id="71907-147">templateId</span><span class="sxs-lookup"><span data-stu-id="71907-147">templateId</span></span>|<span data-ttu-id="71907-148">String</span><span class="sxs-lookup"><span data-stu-id="71907-148">String</span></span>|<span data-ttu-id="71907-149">A ID do modelo de que esta intenção foi criada (se houver)</span><span class="sxs-lookup"><span data-stu-id="71907-149">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="71907-150">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71907-150">roleScopeTagIds</span></span>|<span data-ttu-id="71907-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71907-151">String collection</span></span>|<span data-ttu-id="71907-152">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="71907-152">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="71907-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="71907-153">Response</span></span>
<span data-ttu-id="71907-154">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71907-154">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71907-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71907-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="71907-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71907-156">Request</span></span>
<span data-ttu-id="71907-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71907-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71907-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="71907-158">Response</span></span>
<span data-ttu-id="71907-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71907-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




