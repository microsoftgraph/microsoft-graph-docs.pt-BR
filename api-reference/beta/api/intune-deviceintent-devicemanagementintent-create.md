---
title: Criar deviceManagementIntent
description: Criar um novo objeto deviceManagementIntent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2a8e8847e57f9a79367ff848bb02be65ef5ee52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000725"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="f9cf0-103">Criar deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="f9cf0-103">Create deviceManagementIntent</span></span>

<span data-ttu-id="f9cf0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9cf0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9cf0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9cf0-107">Criar um novo objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="f9cf0-107">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9cf0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9cf0-108">Prerequisites</span></span>
<span data-ttu-id="f9cf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9cf0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9cf0-111">Permission type</span></span>|<span data-ttu-id="f9cf0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9cf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9cf0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9cf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9cf0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9cf0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9cf0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9cf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9cf0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-116">Not supported.</span></span>|
|<span data-ttu-id="f9cf0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9cf0-117">Application</span></span>|<span data-ttu-id="f9cf0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9cf0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9cf0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9cf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="f9cf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf0-120">Request headers</span></span>
|<span data-ttu-id="f9cf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9cf0-121">Header</span></span>|<span data-ttu-id="f9cf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9cf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9cf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9cf0-123">Authorization</span></span>|<span data-ttu-id="f9cf0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9cf0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9cf0-125">Accept</span></span>|<span data-ttu-id="f9cf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9cf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9cf0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf0-127">Request body</span></span>
<span data-ttu-id="f9cf0-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-128">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="f9cf0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-129">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="f9cf0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9cf0-130">Property</span></span>|<span data-ttu-id="f9cf0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9cf0-131">Type</span></span>|<span data-ttu-id="f9cf0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9cf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9cf0-133">id</span><span class="sxs-lookup"><span data-stu-id="f9cf0-133">id</span></span>|<span data-ttu-id="f9cf0-134">String</span><span class="sxs-lookup"><span data-stu-id="f9cf0-134">String</span></span>|<span data-ttu-id="f9cf0-135">A ID de intenção</span><span class="sxs-lookup"><span data-stu-id="f9cf0-135">The intent ID</span></span>|
|<span data-ttu-id="f9cf0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f9cf0-136">displayName</span></span>|<span data-ttu-id="f9cf0-137">String</span><span class="sxs-lookup"><span data-stu-id="f9cf0-137">String</span></span>|<span data-ttu-id="f9cf0-138">O nome de exibição fornecido pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f9cf0-138">The user given display name</span></span>|
|<span data-ttu-id="f9cf0-139">description</span><span class="sxs-lookup"><span data-stu-id="f9cf0-139">description</span></span>|<span data-ttu-id="f9cf0-140">String</span><span class="sxs-lookup"><span data-stu-id="f9cf0-140">String</span></span>|<span data-ttu-id="f9cf0-141">Descrição fornecida pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f9cf0-141">The user given description</span></span>|
|<span data-ttu-id="f9cf0-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f9cf0-142">isAssigned</span></span>|<span data-ttu-id="f9cf0-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9cf0-143">Boolean</span></span>|<span data-ttu-id="f9cf0-144">Significa se a intenção é atribuída ou não aos usuários</span><span class="sxs-lookup"><span data-stu-id="f9cf0-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="f9cf0-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9cf0-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f9cf0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9cf0-146">DateTimeOffset</span></span>|<span data-ttu-id="f9cf0-147">Quando a intenção foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="f9cf0-147">When the intent was last modified</span></span>|
|<span data-ttu-id="f9cf0-148">templateId</span><span class="sxs-lookup"><span data-stu-id="f9cf0-148">templateId</span></span>|<span data-ttu-id="f9cf0-149">String</span><span class="sxs-lookup"><span data-stu-id="f9cf0-149">String</span></span>|<span data-ttu-id="f9cf0-150">A ID do modelo de que esta intenção foi criada (se houver)</span><span class="sxs-lookup"><span data-stu-id="f9cf0-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="f9cf0-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9cf0-151">roleScopeTagIds</span></span>|<span data-ttu-id="f9cf0-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9cf0-152">String collection</span></span>|<span data-ttu-id="f9cf0-153">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f9cf0-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cf0-154">Response</span></span>
<span data-ttu-id="f9cf0-155">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9cf0-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9cf0-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9cf0-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9cf0-157">Request</span></span>
<span data-ttu-id="f9cf0-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9cf0-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9cf0-159">Response</span></span>
<span data-ttu-id="f9cf0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9cf0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






