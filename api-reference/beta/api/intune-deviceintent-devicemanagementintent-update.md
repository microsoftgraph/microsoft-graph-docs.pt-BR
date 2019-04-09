---
title: Atualizar deviceManagementIntent
description: Atualiza as propriedades de um objeto deviceManagementIntent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d73b31e74b56355e46f79ff9c5961f605f2f4fc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523977"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="e8f9a-103">Atualizar deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="e8f9a-103">Update deviceManagementIntent</span></span>

> <span data-ttu-id="e8f9a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f9a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f9a-106">Atualiza as propriedades de um objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="e8f9a-106">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8f9a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8f9a-107">Prerequisites</span></span>
<span data-ttu-id="e8f9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f9a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8f9a-110">Permission type</span></span>|<span data-ttu-id="e8f9a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8f9a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f9a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8f9a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f9a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8f9a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8f9a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8f9a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f9a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-115">Not supported.</span></span>|
|<span data-ttu-id="e8f9a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8f9a-116">Application</span></span>|<span data-ttu-id="e8f9a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f9a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8f9a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="e8f9a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f9a-119">Request headers</span></span>
|<span data-ttu-id="e8f9a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8f9a-120">Header</span></span>|<span data-ttu-id="e8f9a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e8f9a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f9a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8f9a-122">Authorization</span></span>|<span data-ttu-id="e8f9a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f9a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8f9a-124">Accept</span></span>|<span data-ttu-id="e8f9a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f9a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f9a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f9a-126">Request body</span></span>
<span data-ttu-id="e8f9a-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) .</span><span class="sxs-lookup"><span data-stu-id="e8f9a-127">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="e8f9a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span><span class="sxs-lookup"><span data-stu-id="e8f9a-128">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="e8f9a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8f9a-129">Property</span></span>|<span data-ttu-id="e8f9a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8f9a-130">Type</span></span>|<span data-ttu-id="e8f9a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8f9a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8f9a-132">id</span><span class="sxs-lookup"><span data-stu-id="e8f9a-132">id</span></span>|<span data-ttu-id="e8f9a-133">String</span><span class="sxs-lookup"><span data-stu-id="e8f9a-133">String</span></span>|<span data-ttu-id="e8f9a-134">A ID de intenção</span><span class="sxs-lookup"><span data-stu-id="e8f9a-134">The intent ID</span></span>|
|<span data-ttu-id="e8f9a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e8f9a-135">displayName</span></span>|<span data-ttu-id="e8f9a-136">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e8f9a-136">String</span></span>|<span data-ttu-id="e8f9a-137">O nome de exibição fornecido pelo usuário</span><span class="sxs-lookup"><span data-stu-id="e8f9a-137">The user given display name</span></span>|
|<span data-ttu-id="e8f9a-138">description</span><span class="sxs-lookup"><span data-stu-id="e8f9a-138">description</span></span>|<span data-ttu-id="e8f9a-139">String</span><span class="sxs-lookup"><span data-stu-id="e8f9a-139">String</span></span>|<span data-ttu-id="e8f9a-140">Descrição fornecida pelo usuário</span><span class="sxs-lookup"><span data-stu-id="e8f9a-140">The user given description</span></span>|
|<span data-ttu-id="e8f9a-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e8f9a-141">isAssigned</span></span>|<span data-ttu-id="e8f9a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8f9a-142">Boolean</span></span>|<span data-ttu-id="e8f9a-143">Significa se a intenção é atribuída ou não aos usuários</span><span class="sxs-lookup"><span data-stu-id="e8f9a-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="e8f9a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8f9a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="e8f9a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8f9a-145">DateTimeOffset</span></span>|<span data-ttu-id="e8f9a-146">Quando a intenção foi modificada pela última vez</span><span class="sxs-lookup"><span data-stu-id="e8f9a-146">When the intent was last modified</span></span>|
|<span data-ttu-id="e8f9a-147">templateId</span><span class="sxs-lookup"><span data-stu-id="e8f9a-147">templateId</span></span>|<span data-ttu-id="e8f9a-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="e8f9a-148">String</span></span>|<span data-ttu-id="e8f9a-149">A ID do modelo de que esta intenção foi criada (se houver)</span><span class="sxs-lookup"><span data-stu-id="e8f9a-149">The ID of the template this intent was created from (if any)</span></span>|



## <a name="response"></a><span data-ttu-id="e8f9a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f9a-150">Response</span></span>
<span data-ttu-id="e8f9a-151">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8f9a-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8f9a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8f9a-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8f9a-153">Request</span></span>
<span data-ttu-id="e8f9a-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
Content-type: application/json
Content-length: 204

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value"
}
```

### <a name="response"></a><span data-ttu-id="e8f9a-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8f9a-155">Response</span></span>
<span data-ttu-id="e8f9a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8f9a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value"
}
```







