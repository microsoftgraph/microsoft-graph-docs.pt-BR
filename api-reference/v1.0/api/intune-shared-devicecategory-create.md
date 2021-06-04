---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 233046ca0eb9a03c6b43cc58b4c4bf83a90878d8
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732250"
---
# <a name="create-devicecategory"></a><span data-ttu-id="a3580-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="a3580-103">Create deviceCategory</span></span>

<span data-ttu-id="a3580-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3580-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3580-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a3580-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3580-106">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="a3580-106">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3580-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3580-107">Prerequisites</span></span>
<span data-ttu-id="a3580-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3580-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3580-110">Permission type</span></span>|<span data-ttu-id="a3580-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3580-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3580-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3580-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a3580-113">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="a3580-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a3580-114">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3580-114">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3580-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3580-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3580-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3580-116">Not supported.</span></span>|
|<span data-ttu-id="a3580-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3580-117">Application</span></span>|<span data-ttu-id="a3580-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3580-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3580-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3580-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="a3580-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3580-120">Request headers</span></span>
|<span data-ttu-id="a3580-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3580-121">Header</span></span>|<span data-ttu-id="a3580-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a3580-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3580-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3580-123">Authorization</span></span>|<span data-ttu-id="a3580-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3580-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3580-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a3580-125">Accept</span></span>|<span data-ttu-id="a3580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3580-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3580-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3580-127">Request body</span></span>
<span data-ttu-id="a3580-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="a3580-128">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="a3580-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="a3580-129">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="a3580-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3580-130">Property</span></span>|<span data-ttu-id="a3580-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3580-131">Type</span></span>|<span data-ttu-id="a3580-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3580-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3580-133">id</span><span class="sxs-lookup"><span data-stu-id="a3580-133">id</span></span>|<span data-ttu-id="a3580-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3580-134">String</span></span>|<span data-ttu-id="a3580-135">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a3580-135">Unique identifier for the device category.</span></span> <span data-ttu-id="a3580-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3580-136">Read-only.</span></span>|
|<span data-ttu-id="a3580-137">**Integração**</span><span class="sxs-lookup"><span data-stu-id="a3580-137">**Onboarding**</span></span>|
|<span data-ttu-id="a3580-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a3580-138">displayName</span></span>|<span data-ttu-id="a3580-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3580-139">String</span></span>|<span data-ttu-id="a3580-140">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a3580-140">Display name for the device category.</span></span>|
|<span data-ttu-id="a3580-141">descrição</span><span class="sxs-lookup"><span data-stu-id="a3580-141">description</span></span>|<span data-ttu-id="a3580-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3580-142">String</span></span>|<span data-ttu-id="a3580-143">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a3580-143">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="a3580-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3580-144">Response</span></span>
<span data-ttu-id="a3580-145">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3580-145">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3580-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3580-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3580-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3580-147">Request</span></span>
<span data-ttu-id="a3580-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3580-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3580-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3580-149">Response</span></span>
<span data-ttu-id="a3580-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3580-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









