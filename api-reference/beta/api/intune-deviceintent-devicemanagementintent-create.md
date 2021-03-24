---
title: Criar deviceManagementIntent
description: Crie um novo objeto deviceManagementIntent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 20cb05e52b7b065f2cbf1768895e9686bd4a49d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128912"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="38fb4-103">Criar deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="38fb4-103">Create deviceManagementIntent</span></span>

<span data-ttu-id="38fb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38fb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38fb4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38fb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38fb4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38fb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38fb4-107">Crie um novo [objeto deviceManagementIntent.](../resources/intune-deviceintent-devicemanagementintent.md)</span><span class="sxs-lookup"><span data-stu-id="38fb4-107">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38fb4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38fb4-108">Prerequisites</span></span>
<span data-ttu-id="38fb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38fb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38fb4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38fb4-111">Permission type</span></span>|<span data-ttu-id="38fb4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38fb4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38fb4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38fb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38fb4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38fb4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38fb4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38fb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38fb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38fb4-116">Not supported.</span></span>|
|<span data-ttu-id="38fb4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38fb4-117">Application</span></span>|<span data-ttu-id="38fb4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38fb4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38fb4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38fb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="38fb4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38fb4-120">Request headers</span></span>
|<span data-ttu-id="38fb4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38fb4-121">Header</span></span>|<span data-ttu-id="38fb4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="38fb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38fb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38fb4-123">Authorization</span></span>|<span data-ttu-id="38fb4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38fb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38fb4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38fb4-125">Accept</span></span>|<span data-ttu-id="38fb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38fb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38fb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38fb4-127">Request body</span></span>
<span data-ttu-id="38fb4-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="38fb4-128">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="38fb4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementIntent.</span><span class="sxs-lookup"><span data-stu-id="38fb4-129">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="38fb4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38fb4-130">Property</span></span>|<span data-ttu-id="38fb4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="38fb4-131">Type</span></span>|<span data-ttu-id="38fb4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="38fb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38fb4-133">id</span><span class="sxs-lookup"><span data-stu-id="38fb4-133">id</span></span>|<span data-ttu-id="38fb4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38fb4-134">String</span></span>|<span data-ttu-id="38fb4-135">A ID de intenção</span><span class="sxs-lookup"><span data-stu-id="38fb4-135">The intent ID</span></span>|
|<span data-ttu-id="38fb4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="38fb4-136">displayName</span></span>|<span data-ttu-id="38fb4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38fb4-137">String</span></span>|<span data-ttu-id="38fb4-138">O nome de exibição dado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="38fb4-138">The user given display name</span></span>|
|<span data-ttu-id="38fb4-139">descrição</span><span class="sxs-lookup"><span data-stu-id="38fb4-139">description</span></span>|<span data-ttu-id="38fb4-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38fb4-140">String</span></span>|<span data-ttu-id="38fb4-141">A descrição dada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="38fb4-141">The user given description</span></span>|
|<span data-ttu-id="38fb4-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="38fb4-142">isAssigned</span></span>|<span data-ttu-id="38fb4-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="38fb4-143">Boolean</span></span>|<span data-ttu-id="38fb4-144">Significa se a intenção é atribuída ou não aos usuários</span><span class="sxs-lookup"><span data-stu-id="38fb4-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="38fb4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38fb4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="38fb4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38fb4-146">DateTimeOffset</span></span>|<span data-ttu-id="38fb4-147">Quando a intenção foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="38fb4-147">When the intent was last modified</span></span>|
|<span data-ttu-id="38fb4-148">templateId</span><span class="sxs-lookup"><span data-stu-id="38fb4-148">templateId</span></span>|<span data-ttu-id="38fb4-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38fb4-149">String</span></span>|<span data-ttu-id="38fb4-150">A ID do modelo de que essa intenção foi criada (se alguma)</span><span class="sxs-lookup"><span data-stu-id="38fb4-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="38fb4-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38fb4-151">roleScopeTagIds</span></span>|<span data-ttu-id="38fb4-152">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="38fb4-152">String collection</span></span>|<span data-ttu-id="38fb4-153">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="38fb4-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="38fb4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="38fb4-154">Response</span></span>
<span data-ttu-id="38fb4-155">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38fb4-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38fb4-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38fb4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="38fb4-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38fb4-157">Request</span></span>
<span data-ttu-id="38fb4-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38fb4-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38fb4-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="38fb4-159">Response</span></span>
<span data-ttu-id="38fb4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38fb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




