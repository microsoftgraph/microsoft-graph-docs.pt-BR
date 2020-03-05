---
title: Criar sideLoadingKey
description: Criar um novo objeto sideLoadingKey.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3517b299f2a6d97bba08f49a88dbefa7c393c78f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42461834"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="30fde-103">Criar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="30fde-103">Create sideLoadingKey</span></span>

<span data-ttu-id="30fde-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="30fde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30fde-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30fde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30fde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30fde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30fde-107">Criar um novo objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="30fde-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30fde-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30fde-108">Prerequisites</span></span>
<span data-ttu-id="30fde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30fde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30fde-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30fde-111">Permission type</span></span>|<span data-ttu-id="30fde-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30fde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30fde-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30fde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30fde-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30fde-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="30fde-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30fde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30fde-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30fde-116">Not supported.</span></span>|
|<span data-ttu-id="30fde-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30fde-117">Application</span></span>|<span data-ttu-id="30fde-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30fde-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30fde-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30fde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="30fde-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30fde-120">Request headers</span></span>
|<span data-ttu-id="30fde-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30fde-121">Header</span></span>|<span data-ttu-id="30fde-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30fde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30fde-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30fde-123">Authorization</span></span>|<span data-ttu-id="30fde-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30fde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30fde-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30fde-125">Accept</span></span>|<span data-ttu-id="30fde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30fde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30fde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30fde-127">Request body</span></span>
<span data-ttu-id="30fde-128">No corpo da solicitação, forneça uma representação JSON do objeto sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="30fde-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="30fde-129">A tabela a seguir mostra as propriedades que são necessárias ao criar sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="30fde-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="30fde-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30fde-130">Property</span></span>|<span data-ttu-id="30fde-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30fde-131">Type</span></span>|<span data-ttu-id="30fde-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30fde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30fde-133">id</span><span class="sxs-lookup"><span data-stu-id="30fde-133">id</span></span>|<span data-ttu-id="30fde-134">String</span><span class="sxs-lookup"><span data-stu-id="30fde-134">String</span></span>|<span data-ttu-id="30fde-135">ID exclusiva da chave de carregamento do lado.</span><span class="sxs-lookup"><span data-stu-id="30fde-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="30fde-136">value</span><span class="sxs-lookup"><span data-stu-id="30fde-136">value</span></span>|<span data-ttu-id="30fde-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30fde-137">String</span></span>|<span data-ttu-id="30fde-138">O valor da chave de carregamento do lado, é o valor de 5x5, separado por hiphens.</span><span class="sxs-lookup"><span data-stu-id="30fde-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="30fde-139">displayName</span><span class="sxs-lookup"><span data-stu-id="30fde-139">displayName</span></span>|<span data-ttu-id="30fde-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30fde-140">String</span></span>|<span data-ttu-id="30fde-141">Nome da chave de carregamento do lado exibido para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="30fde-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="30fde-142">description</span><span class="sxs-lookup"><span data-stu-id="30fde-142">description</span></span>|<span data-ttu-id="30fde-143">String</span><span class="sxs-lookup"><span data-stu-id="30fde-143">String</span></span>|<span data-ttu-id="30fde-144">Descrição da chave de carregamento do lado exibida para os administradores do profissionais..</span><span class="sxs-lookup"><span data-stu-id="30fde-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="30fde-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="30fde-145">totalActivation</span></span>|<span data-ttu-id="30fde-146">Int32</span><span class="sxs-lookup"><span data-stu-id="30fde-146">Int32</span></span>|<span data-ttu-id="30fde-147">Chave de carregamento do lado ativação total exibida para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="30fde-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="30fde-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="30fde-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="30fde-149">String</span><span class="sxs-lookup"><span data-stu-id="30fde-149">String</span></span>|<span data-ttu-id="30fde-150">Chave de carregamento lateral última data de atualização exibida para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="30fde-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="30fde-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="30fde-151">Response</span></span>
<span data-ttu-id="30fde-152">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30fde-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30fde-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30fde-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="30fde-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30fde-154">Request</span></span>
<span data-ttu-id="30fde-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30fde-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30fde-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="30fde-156">Response</span></span>
<span data-ttu-id="30fde-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30fde-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





