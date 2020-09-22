---
title: Criar sideLoadingKey
description: Criar um novo objeto sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5283c555cdf111c8651173574634cbdb6fc9bafe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032177"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="ab839-103">Criar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="ab839-103">Create sideLoadingKey</span></span>

<span data-ttu-id="ab839-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab839-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab839-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab839-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab839-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab839-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab839-107">Criar um novo objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="ab839-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab839-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab839-108">Prerequisites</span></span>
<span data-ttu-id="ab839-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab839-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab839-111">Permission type</span></span>|<span data-ttu-id="ab839-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab839-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab839-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab839-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab839-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab839-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab839-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab839-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab839-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab839-116">Not supported.</span></span>|
|<span data-ttu-id="ab839-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab839-117">Application</span></span>|<span data-ttu-id="ab839-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab839-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab839-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab839-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="ab839-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab839-120">Request headers</span></span>
|<span data-ttu-id="ab839-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab839-121">Header</span></span>|<span data-ttu-id="ab839-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ab839-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab839-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab839-123">Authorization</span></span>|<span data-ttu-id="ab839-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab839-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab839-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab839-125">Accept</span></span>|<span data-ttu-id="ab839-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab839-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab839-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab839-127">Request body</span></span>
<span data-ttu-id="ab839-128">No corpo da solicitação, forneça uma representação JSON do objeto sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="ab839-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="ab839-129">A tabela a seguir mostra as propriedades que são necessárias ao criar sideLoadingKey.</span><span class="sxs-lookup"><span data-stu-id="ab839-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="ab839-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab839-130">Property</span></span>|<span data-ttu-id="ab839-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab839-131">Type</span></span>|<span data-ttu-id="ab839-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab839-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab839-133">id</span><span class="sxs-lookup"><span data-stu-id="ab839-133">id</span></span>|<span data-ttu-id="ab839-134">String</span><span class="sxs-lookup"><span data-stu-id="ab839-134">String</span></span>|<span data-ttu-id="ab839-135">ID exclusiva da chave de carregamento do lado.</span><span class="sxs-lookup"><span data-stu-id="ab839-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="ab839-136">value</span><span class="sxs-lookup"><span data-stu-id="ab839-136">value</span></span>|<span data-ttu-id="ab839-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab839-137">String</span></span>|<span data-ttu-id="ab839-138">O valor da chave de carregamento do lado, é o valor de 5x5, separado por hiphens.</span><span class="sxs-lookup"><span data-stu-id="ab839-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="ab839-139">displayName</span><span class="sxs-lookup"><span data-stu-id="ab839-139">displayName</span></span>|<span data-ttu-id="ab839-140">String</span><span class="sxs-lookup"><span data-stu-id="ab839-140">String</span></span>|<span data-ttu-id="ab839-141">Nome da chave de carregamento do lado exibido para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="ab839-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ab839-142">description</span><span class="sxs-lookup"><span data-stu-id="ab839-142">description</span></span>|<span data-ttu-id="ab839-143">String</span><span class="sxs-lookup"><span data-stu-id="ab839-143">String</span></span>|<span data-ttu-id="ab839-144">Descrição da chave de carregamento do lado exibida para os administradores do profissionais..</span><span class="sxs-lookup"><span data-stu-id="ab839-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="ab839-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="ab839-145">totalActivation</span></span>|<span data-ttu-id="ab839-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ab839-146">Int32</span></span>|<span data-ttu-id="ab839-147">Chave de carregamento do lado ativação total exibida para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="ab839-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="ab839-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab839-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="ab839-149">String</span><span class="sxs-lookup"><span data-stu-id="ab839-149">String</span></span>|<span data-ttu-id="ab839-150">Chave de carregamento lateral última data de atualização exibida para os administradores do profissionais.</span><span class="sxs-lookup"><span data-stu-id="ab839-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="ab839-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab839-151">Response</span></span>
<span data-ttu-id="ab839-152">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab839-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab839-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab839-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab839-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab839-154">Request</span></span>
<span data-ttu-id="ab839-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab839-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab839-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab839-156">Response</span></span>
<span data-ttu-id="ab839-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab839-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






