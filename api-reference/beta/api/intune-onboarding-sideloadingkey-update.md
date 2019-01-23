---
title: Atualizar sideLoadingKey
description: Atualize as propriedades de um objeto sideLoadingKey.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fd498404543353c45714f739a68b0195ae3d3dd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409857"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="9f2c0-103">Atualizar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="9f2c0-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="9f2c0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f2c0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f2c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f2c0-107">Atualize as propriedades de um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="9f2c0-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f2c0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f2c0-108">Prerequisites</span></span>
<span data-ttu-id="9f2c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f2c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f2c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f2c0-111">Permission type</span></span>|<span data-ttu-id="9f2c0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f2c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f2c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f2c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f2c0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f2c0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f2c0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f2c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f2c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-116">Not supported.</span></span>|
|<span data-ttu-id="9f2c0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f2c0-117">Application</span></span>|<span data-ttu-id="9f2c0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f2c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f2c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="9f2c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f2c0-120">Request headers</span></span>
|<span data-ttu-id="9f2c0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f2c0-121">Header</span></span>|<span data-ttu-id="9f2c0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9f2c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f2c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f2c0-123">Authorization</span></span>|<span data-ttu-id="9f2c0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f2c0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f2c0-125">Accept</span></span>|<span data-ttu-id="9f2c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f2c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f2c0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f2c0-127">Request body</span></span>
<span data-ttu-id="9f2c0-128">No corpo da solicitação, fornece uma representação JSON para o objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="9f2c0-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="9f2c0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="9f2c0-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="9f2c0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f2c0-130">Property</span></span>|<span data-ttu-id="9f2c0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f2c0-131">Type</span></span>|<span data-ttu-id="9f2c0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f2c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f2c0-133">id</span><span class="sxs-lookup"><span data-stu-id="9f2c0-133">id</span></span>|<span data-ttu-id="9f2c0-134">String</span><span class="sxs-lookup"><span data-stu-id="9f2c0-134">String</span></span>|<span data-ttu-id="9f2c0-135">Lado carregando o ID exclusivo principal.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="9f2c0-136">valor</span><span class="sxs-lookup"><span data-stu-id="9f2c0-136">value</span></span>|<span data-ttu-id="9f2c0-137">String</span><span class="sxs-lookup"><span data-stu-id="9f2c0-137">String</span></span>|<span data-ttu-id="9f2c0-138">Valor da chave Carregando lado, é 5x5 valor, separados por hiphens.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="9f2c0-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9f2c0-139">displayName</span></span>|<span data-ttu-id="9f2c0-140">String</span><span class="sxs-lookup"><span data-stu-id="9f2c0-140">String</span></span>|<span data-ttu-id="9f2c0-141">Carregando da lado chave nome exibido para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9f2c0-142">description</span><span class="sxs-lookup"><span data-stu-id="9f2c0-142">description</span></span>|<span data-ttu-id="9f2c0-143">String</span><span class="sxs-lookup"><span data-stu-id="9f2c0-143">String</span></span>|<span data-ttu-id="9f2c0-144">Descrição de chave Carregando lado exibida para o ITPro Admins..</span><span class="sxs-lookup"><span data-stu-id="9f2c0-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="9f2c0-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="9f2c0-145">totalActivation</span></span>|<span data-ttu-id="9f2c0-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9f2c0-146">Int32</span></span>|<span data-ttu-id="9f2c0-147">Lado Carregando chave Total Activation exibida para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9f2c0-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f2c0-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="9f2c0-149">String</span><span class="sxs-lookup"><span data-stu-id="9f2c0-149">String</span></span>|<span data-ttu-id="9f2c0-150">Lado Carregando chave última atualizado data exibida para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="9f2c0-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f2c0-151">Response</span></span>
<span data-ttu-id="9f2c0-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f2c0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f2c0-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f2c0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f2c0-154">Request</span></span>
<span data-ttu-id="9f2c0-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f2c0-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f2c0-156">Response</span></span>
<span data-ttu-id="9f2c0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f2c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




