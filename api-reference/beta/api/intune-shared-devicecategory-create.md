---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bbe00ccf9d94b9cc9253ad1baeeaedbaec29734d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458859"
---
# <a name="create-devicecategory"></a><span data-ttu-id="21c7f-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="21c7f-103">Create deviceCategory</span></span>

<span data-ttu-id="21c7f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="21c7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21c7f-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="21c7f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21c7f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="21c7f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21c7f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21c7f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21c7f-108">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="21c7f-108">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21c7f-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21c7f-109">Prerequisites</span></span>

<span data-ttu-id="21c7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21c7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21c7f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21c7f-112">Permission type</span></span>|<span data-ttu-id="21c7f-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21c7f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21c7f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21c7f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="21c7f-115">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="21c7f-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="21c7f-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21c7f-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="21c7f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21c7f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21c7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21c7f-118">Not supported.</span></span>|
|<span data-ttu-id="21c7f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21c7f-119">Application</span></span>||
| <span data-ttu-id="21c7f-120">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="21c7f-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="21c7f-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21c7f-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21c7f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21c7f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="21c7f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21c7f-123">Request headers</span></span>

|<span data-ttu-id="21c7f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21c7f-124">Header</span></span>|<span data-ttu-id="21c7f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="21c7f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21c7f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="21c7f-126">Authorization</span></span>|<span data-ttu-id="21c7f-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21c7f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21c7f-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21c7f-128">Accept</span></span>|<span data-ttu-id="21c7f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="21c7f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21c7f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21c7f-130">Request body</span></span>

<span data-ttu-id="21c7f-131">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="21c7f-131">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="21c7f-132">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="21c7f-132">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="21c7f-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21c7f-133">Property</span></span>|<span data-ttu-id="21c7f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="21c7f-134">Type</span></span>|<span data-ttu-id="21c7f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="21c7f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21c7f-136">id</span><span class="sxs-lookup"><span data-stu-id="21c7f-136">id</span></span>|<span data-ttu-id="21c7f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21c7f-137">String</span></span>|<span data-ttu-id="21c7f-138">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21c7f-138">Unique identifier for the device category.</span></span> <span data-ttu-id="21c7f-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="21c7f-139">Read-only.</span></span>|
|<span data-ttu-id="21c7f-140">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="21c7f-140">**Obboarding**</span></span>|
|<span data-ttu-id="21c7f-141">description</span><span class="sxs-lookup"><span data-stu-id="21c7f-141">description</span></span>|<span data-ttu-id="21c7f-142">String</span><span class="sxs-lookup"><span data-stu-id="21c7f-142">String</span></span>|<span data-ttu-id="21c7f-143">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21c7f-143">Optional description for the device category.</span></span>|
|<span data-ttu-id="21c7f-144">displayName</span><span class="sxs-lookup"><span data-stu-id="21c7f-144">displayName</span></span>|<span data-ttu-id="21c7f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21c7f-145">String</span></span>|<span data-ttu-id="21c7f-146">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21c7f-146">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="21c7f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c7f-147">Response</span></span>

<span data-ttu-id="21c7f-148">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21c7f-148">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21c7f-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21c7f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="21c7f-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21c7f-150">Request</span></span>

<span data-ttu-id="21c7f-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21c7f-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="21c7f-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="21c7f-152">Response</span></span>

<span data-ttu-id="21c7f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21c7f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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











