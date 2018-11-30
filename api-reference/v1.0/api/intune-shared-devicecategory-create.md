---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
ms.openlocfilehash: 43a731716150a7cc9515a6497840cc47271e88c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005919"
---
# <a name="create-devicecategory"></a><span data-ttu-id="f1b3a-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="f1b3a-103">Create deviceCategory</span></span>

> <span data-ttu-id="f1b3a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1b3a-105">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="f1b3a-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1b3a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1b3a-106">Prerequisites</span></span>
<span data-ttu-id="f1b3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1b3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1b3a-109">Permission type</span></span>|<span data-ttu-id="f1b3a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1b3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1b3a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1b3a-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f1b3a-112">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="f1b3a-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f1b3a-113">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b3a-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="f1b3a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1b3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1b3a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-115">Not supported.</span></span>|
|<span data-ttu-id="f1b3a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1b3a-116">Application</span></span>|<span data-ttu-id="f1b3a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1b3a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1b3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="f1b3a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b3a-119">Request headers</span></span>
|<span data-ttu-id="f1b3a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1b3a-120">Header</span></span>|<span data-ttu-id="f1b3a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1b3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1b3a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1b3a-122">Authorization</span></span>|<span data-ttu-id="f1b3a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1b3a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f1b3a-124">Accept</span></span>|<span data-ttu-id="f1b3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1b3a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b3a-126">Request body</span></span>
<span data-ttu-id="f1b3a-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="f1b3a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="f1b3a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1b3a-129">Property</span></span>|<span data-ttu-id="f1b3a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1b3a-130">Type</span></span>|<span data-ttu-id="f1b3a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b3a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1b3a-132">id</span><span class="sxs-lookup"><span data-stu-id="f1b3a-132">id</span></span>|<span data-ttu-id="f1b3a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b3a-133">String</span></span>|<span data-ttu-id="f1b3a-134">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-134">Unique identifier for the device category.</span></span> <span data-ttu-id="f1b3a-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-135">Read-only.</span></span>|
|<span data-ttu-id="f1b3a-136">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="f1b3a-136">**Onboarding**</span></span>|
|<span data-ttu-id="f1b3a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f1b3a-137">displayName</span></span>|<span data-ttu-id="f1b3a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b3a-138">String</span></span>|<span data-ttu-id="f1b3a-139">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-139">Display name for the device category.</span></span>|
|<span data-ttu-id="f1b3a-140">description</span><span class="sxs-lookup"><span data-stu-id="f1b3a-140">description</span></span>|<span data-ttu-id="f1b3a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1b3a-141">String</span></span>|<span data-ttu-id="f1b3a-142">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="f1b3a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b3a-143">Response</span></span>
<span data-ttu-id="f1b3a-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1b3a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1b3a-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1b3a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1b3a-146">Request</span></span>
<span data-ttu-id="f1b3a-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f1b3a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1b3a-148">Response</span></span>
<span data-ttu-id="f1b3a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1b3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



