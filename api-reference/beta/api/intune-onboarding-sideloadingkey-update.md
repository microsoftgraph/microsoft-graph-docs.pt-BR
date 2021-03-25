---
title: Atualizar sideLoadingKey
description: Atualize as propriedades de um objeto sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65ae9cfcb7fd2d66c8b56108929a284f26d840fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152667"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="9b7ef-103">Atualizar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="9b7ef-103">Update sideLoadingKey</span></span>

<span data-ttu-id="9b7ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b7ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b7ef-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b7ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b7ef-107">Atualize as propriedades de um [objeto sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="9b7ef-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b7ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9b7ef-108">Prerequisites</span></span>
<span data-ttu-id="9b7ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b7ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b7ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b7ef-111">Permission type</span></span>|<span data-ttu-id="9b7ef-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b7ef-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b7ef-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b7ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b7ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b7ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9b7ef-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b7ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b7ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-116">Not supported.</span></span>|
|<span data-ttu-id="9b7ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b7ef-117">Application</span></span>|<span data-ttu-id="9b7ef-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b7ef-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b7ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b7ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="9b7ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b7ef-120">Request headers</span></span>
|<span data-ttu-id="9b7ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9b7ef-121">Header</span></span>|<span data-ttu-id="9b7ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9b7ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b7ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b7ef-123">Authorization</span></span>|<span data-ttu-id="9b7ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b7ef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9b7ef-125">Accept</span></span>|<span data-ttu-id="9b7ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b7ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b7ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b7ef-127">Request body</span></span>
<span data-ttu-id="9b7ef-128">No corpo da solicitação, fornece uma representação JSON para o [objeto sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)</span><span class="sxs-lookup"><span data-stu-id="9b7ef-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="9b7ef-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="9b7ef-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="9b7ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b7ef-130">Property</span></span>|<span data-ttu-id="9b7ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b7ef-131">Type</span></span>|<span data-ttu-id="9b7ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b7ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b7ef-133">id</span><span class="sxs-lookup"><span data-stu-id="9b7ef-133">id</span></span>|<span data-ttu-id="9b7ef-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b7ef-134">String</span></span>|<span data-ttu-id="9b7ef-135">ID exclusiva da chave de carregamento lateral.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="9b7ef-136">value</span><span class="sxs-lookup"><span data-stu-id="9b7ef-136">value</span></span>|<span data-ttu-id="9b7ef-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b7ef-137">String</span></span>|<span data-ttu-id="9b7ef-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="9b7ef-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9b7ef-139">displayName</span></span>|<span data-ttu-id="9b7ef-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b7ef-140">String</span></span>|<span data-ttu-id="9b7ef-141">Side Loading Key Name displayed to the ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9b7ef-142">descrição</span><span class="sxs-lookup"><span data-stu-id="9b7ef-142">description</span></span>|<span data-ttu-id="9b7ef-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b7ef-143">String</span></span>|<span data-ttu-id="9b7ef-144">Descrição da Chave de Carregamento lateral exibida para os administradores do ITPro..</span><span class="sxs-lookup"><span data-stu-id="9b7ef-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="9b7ef-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="9b7ef-145">totalActivation</span></span>|<span data-ttu-id="9b7ef-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9b7ef-146">Int32</span></span>|<span data-ttu-id="9b7ef-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9b7ef-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b7ef-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="9b7ef-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b7ef-149">String</span></span>|<span data-ttu-id="9b7ef-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="9b7ef-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b7ef-151">Response</span></span>
<span data-ttu-id="9b7ef-152">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b7ef-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b7ef-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b7ef-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b7ef-154">Request</span></span>
<span data-ttu-id="9b7ef-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
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

### <a name="response"></a><span data-ttu-id="9b7ef-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b7ef-156">Response</span></span>
<span data-ttu-id="9b7ef-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9b7ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




