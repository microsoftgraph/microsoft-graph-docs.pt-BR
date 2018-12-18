---
title: Atualizar sideLoadingKey
description: Atualize as propriedades de um objeto sideLoadingKey.
author: tfitzmac
ms.openlocfilehash: 6d616db947defb8e08926e40df23590c7d27e84d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337377"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="efa5a-103">Atualizar sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="efa5a-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="efa5a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="efa5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efa5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="efa5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efa5a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="efa5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efa5a-107">Atualize as propriedades de um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="efa5a-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efa5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="efa5a-108">Prerequisites</span></span>
<span data-ttu-id="efa5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efa5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efa5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efa5a-111">Permission type</span></span>|<span data-ttu-id="efa5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="efa5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efa5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efa5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efa5a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efa5a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="efa5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efa5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efa5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efa5a-116">Not supported.</span></span>|
|<span data-ttu-id="efa5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efa5a-117">Application</span></span>|<span data-ttu-id="efa5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efa5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efa5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efa5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="efa5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efa5a-120">Request headers</span></span>
|<span data-ttu-id="efa5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="efa5a-121">Header</span></span>|<span data-ttu-id="efa5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="efa5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efa5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efa5a-123">Authorization</span></span>|<span data-ttu-id="efa5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efa5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efa5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efa5a-125">Accept</span></span>|<span data-ttu-id="efa5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efa5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efa5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efa5a-127">Request body</span></span>
<span data-ttu-id="efa5a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .</span><span class="sxs-lookup"><span data-stu-id="efa5a-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="efa5a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span><span class="sxs-lookup"><span data-stu-id="efa5a-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="efa5a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efa5a-130">Property</span></span>|<span data-ttu-id="efa5a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa5a-131">Type</span></span>|<span data-ttu-id="efa5a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa5a-133">id</span><span class="sxs-lookup"><span data-stu-id="efa5a-133">id</span></span>|<span data-ttu-id="efa5a-134">String</span><span class="sxs-lookup"><span data-stu-id="efa5a-134">String</span></span>|<span data-ttu-id="efa5a-135">Lado carregando o ID exclusivo principal.</span><span class="sxs-lookup"><span data-stu-id="efa5a-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="efa5a-136">valor</span><span class="sxs-lookup"><span data-stu-id="efa5a-136">value</span></span>|<span data-ttu-id="efa5a-137">String</span><span class="sxs-lookup"><span data-stu-id="efa5a-137">String</span></span>|<span data-ttu-id="efa5a-138">Valor da chave Carregando lado, é 5x5 valor, separados por hiphens.</span><span class="sxs-lookup"><span data-stu-id="efa5a-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="efa5a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="efa5a-139">displayName</span></span>|<span data-ttu-id="efa5a-140">String</span><span class="sxs-lookup"><span data-stu-id="efa5a-140">String</span></span>|<span data-ttu-id="efa5a-141">Carregando da lado chave nome exibido para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="efa5a-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="efa5a-142">description</span><span class="sxs-lookup"><span data-stu-id="efa5a-142">description</span></span>|<span data-ttu-id="efa5a-143">String</span><span class="sxs-lookup"><span data-stu-id="efa5a-143">String</span></span>|<span data-ttu-id="efa5a-144">Descrição de chave Carregando lado exibida para o ITPro Admins..</span><span class="sxs-lookup"><span data-stu-id="efa5a-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="efa5a-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="efa5a-145">totalActivation</span></span>|<span data-ttu-id="efa5a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="efa5a-146">Int32</span></span>|<span data-ttu-id="efa5a-147">Lado Carregando chave Total Activation exibida para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="efa5a-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="efa5a-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="efa5a-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="efa5a-149">String</span><span class="sxs-lookup"><span data-stu-id="efa5a-149">String</span></span>|<span data-ttu-id="efa5a-150">Lado Carregando chave última atualizado data exibida para o ITPro Admins.</span><span class="sxs-lookup"><span data-stu-id="efa5a-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="efa5a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa5a-151">Response</span></span>
<span data-ttu-id="efa5a-152">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efa5a-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efa5a-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="efa5a-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="efa5a-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efa5a-154">Request</span></span>
<span data-ttu-id="efa5a-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efa5a-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 193

{
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="efa5a-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="efa5a-156">Response</span></span>
<span data-ttu-id="efa5a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efa5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





