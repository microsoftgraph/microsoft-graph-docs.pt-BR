---
title: Criar sideLoadingKey
description: Criar um novo objeto sideLoadingKey.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be989b909b0d56e6d55c44e3d0df368d5c9c6825
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980723"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="9c1e5-103">Criar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="9c1e5-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="9c1e5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c1e5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c1e5-106">Criar um novo objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="9c1e5-106">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c1e5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c1e5-107">Prerequisites</span></span>
<span data-ttu-id="9c1e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c1e5-110">Permission type</span></span>|<span data-ttu-id="9c1e5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c1e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c1e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1e5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1e5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9c1e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c1e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-115">Not supported.</span></span>|
|<span data-ttu-id="9c1e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c1e5-116">Application</span></span>|<span data-ttu-id="9c1e5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1e5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c1e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="9c1e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1e5-119">Request headers</span></span>
|<span data-ttu-id="9c1e5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c1e5-120">Header</span></span>|<span data-ttu-id="9c1e5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9c1e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1e5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c1e5-122">Authorization</span></span>|<span data-ttu-id="9c1e5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1e5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c1e5-124">Accept</span></span>|<span data-ttu-id="9c1e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1e5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1e5-126">Request body</span></span>
<span data-ttu-id="9c1e5-127">No corpo da solicitação, forneça uma representação JSON do objeto sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-127">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="9c1e5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-128">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="9c1e5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c1e5-129">Property</span></span>|<span data-ttu-id="9c1e5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c1e5-130">Type</span></span>|<span data-ttu-id="9c1e5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c1e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c1e5-132">id</span><span class="sxs-lookup"><span data-stu-id="9c1e5-132">id</span></span>|<span data-ttu-id="9c1e5-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c1e5-133">String</span></span>|<span data-ttu-id="9c1e5-134">ID exclusiva da chave de carregamento do lado.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-134">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="9c1e5-135">value</span><span class="sxs-lookup"><span data-stu-id="9c1e5-135">value</span></span>|<span data-ttu-id="9c1e5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c1e5-136">String</span></span>|<span data-ttu-id="9c1e5-137">O valor da chave de carregamento do lado, é o valor de 5x5, separado por hiphens.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-137">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="9c1e5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9c1e5-138">displayName</span></span>|<span data-ttu-id="9c1e5-139">String</span><span class="sxs-lookup"><span data-stu-id="9c1e5-139">String</span></span>|<span data-ttu-id="9c1e5-140">Nome da chave de carregamento do lado exibido para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-140">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9c1e5-141">descrição</span><span class="sxs-lookup"><span data-stu-id="9c1e5-141">description</span></span>|<span data-ttu-id="9c1e5-142">String</span><span class="sxs-lookup"><span data-stu-id="9c1e5-142">String</span></span>|<span data-ttu-id="9c1e5-143">Descrição da chave de carregamento do lado exibida para os administradores do profissionais..</span><span class="sxs-lookup"><span data-stu-id="9c1e5-143">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="9c1e5-144">totalActivation</span><span class="sxs-lookup"><span data-stu-id="9c1e5-144">totalActivation</span></span>|<span data-ttu-id="9c1e5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1e5-145">Int32</span></span>|<span data-ttu-id="9c1e5-146">Chave de carregamento do lado ativação total exibida para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-146">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9c1e5-147">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c1e5-147">lastUpdatedDateTime</span></span>|<span data-ttu-id="9c1e5-148">String</span><span class="sxs-lookup"><span data-stu-id="9c1e5-148">String</span></span>|<span data-ttu-id="9c1e5-149">Chave de carregamento lateral última data de atualização exibida para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-149">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="9c1e5-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1e5-150">Response</span></span>
<span data-ttu-id="9c1e5-151">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-151">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1e5-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c1e5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c1e5-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c1e5-153">Request</span></span>
<span data-ttu-id="9c1e5-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="9c1e5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c1e5-155">Response</span></span>
<span data-ttu-id="9c1e5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c1e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





