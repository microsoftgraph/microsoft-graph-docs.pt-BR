---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da7ecf3988c83aa7ef7f2fc16ac98271518e3c6b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465806"
---
# <a name="create-devicecategory"></a><span data-ttu-id="2f18f-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2f18f-103">Create deviceCategory</span></span>

<span data-ttu-id="2f18f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f18f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f18f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f18f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f18f-106">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2f18f-106">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f18f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f18f-107">Prerequisites</span></span>
<span data-ttu-id="2f18f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f18f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f18f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f18f-110">Permission type</span></span>|<span data-ttu-id="2f18f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f18f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f18f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f18f-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2f18f-113">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="2f18f-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2f18f-114">Dispositivos DeviceManagementManaged. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2f18f-114">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f18f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f18f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f18f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f18f-116">Not supported.</span></span>|
|<span data-ttu-id="2f18f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f18f-117">Application</span></span>|<span data-ttu-id="2f18f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f18f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f18f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f18f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="2f18f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f18f-120">Request headers</span></span>
|<span data-ttu-id="2f18f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f18f-121">Header</span></span>|<span data-ttu-id="2f18f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f18f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f18f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f18f-123">Authorization</span></span>|<span data-ttu-id="2f18f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f18f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f18f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f18f-125">Accept</span></span>|<span data-ttu-id="2f18f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f18f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f18f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f18f-127">Request body</span></span>
<span data-ttu-id="2f18f-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="2f18f-128">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="2f18f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="2f18f-129">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="2f18f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f18f-130">Property</span></span>|<span data-ttu-id="2f18f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f18f-131">Type</span></span>|<span data-ttu-id="2f18f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f18f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f18f-133">id</span><span class="sxs-lookup"><span data-stu-id="2f18f-133">id</span></span>|<span data-ttu-id="2f18f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f18f-134">String</span></span>|<span data-ttu-id="2f18f-135">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f18f-135">Unique identifier for the device category.</span></span> <span data-ttu-id="2f18f-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f18f-136">Read-only.</span></span>|
|<span data-ttu-id="2f18f-137">**Integração**</span><span class="sxs-lookup"><span data-stu-id="2f18f-137">**Onboarding**</span></span>|
|<span data-ttu-id="2f18f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2f18f-138">displayName</span></span>|<span data-ttu-id="2f18f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f18f-139">String</span></span>|<span data-ttu-id="2f18f-140">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f18f-140">Display name for the device category.</span></span>|
|<span data-ttu-id="2f18f-141">description</span><span class="sxs-lookup"><span data-stu-id="2f18f-141">description</span></span>|<span data-ttu-id="2f18f-142">String</span><span class="sxs-lookup"><span data-stu-id="2f18f-142">String</span></span>|<span data-ttu-id="2f18f-143">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f18f-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="2f18f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f18f-144">Response</span></span>
<span data-ttu-id="2f18f-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f18f-145">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f18f-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f18f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f18f-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f18f-147">Request</span></span>
<span data-ttu-id="2f18f-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f18f-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f18f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f18f-149">Response</span></span>
<span data-ttu-id="2f18f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f18f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






