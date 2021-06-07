---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b1bfb046b4a1949ddba846d5a30c34256198049
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759452"
---
# <a name="create-devicecategory"></a><span data-ttu-id="2ef43-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2ef43-103">Create deviceCategory</span></span>

<span data-ttu-id="2ef43-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ef43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ef43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ef43-106">Cria um novo objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2ef43-106">Create a new [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ef43-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ef43-107">Prerequisites</span></span>
<span data-ttu-id="2ef43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef43-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef43-110">Permission type</span></span>|<span data-ttu-id="2ef43-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ef43-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ef43-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef43-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ef43-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef43-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2ef43-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef43-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ef43-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef43-115">Not supported.</span></span>|
|<span data-ttu-id="2ef43-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef43-116">Application</span></span>|<span data-ttu-id="2ef43-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef43-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ef43-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef43-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="2ef43-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef43-119">Request headers</span></span>
|<span data-ttu-id="2ef43-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ef43-120">Header</span></span>|<span data-ttu-id="2ef43-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ef43-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ef43-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ef43-122">Authorization</span></span>|<span data-ttu-id="2ef43-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef43-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ef43-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ef43-124">Accept</span></span>|<span data-ttu-id="2ef43-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ef43-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ef43-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef43-126">Request body</span></span>
<span data-ttu-id="2ef43-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="2ef43-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="2ef43-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="2ef43-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="2ef43-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ef43-129">Property</span></span>|<span data-ttu-id="2ef43-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ef43-130">Type</span></span>|<span data-ttu-id="2ef43-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef43-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ef43-132">id</span><span class="sxs-lookup"><span data-stu-id="2ef43-132">id</span></span>|<span data-ttu-id="2ef43-133">String</span><span class="sxs-lookup"><span data-stu-id="2ef43-133">String</span></span>|<span data-ttu-id="2ef43-134">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ef43-134">Unique identifier for the device category.</span></span> <span data-ttu-id="2ef43-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ef43-135">Read-only.</span></span>|
|<span data-ttu-id="2ef43-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2ef43-136">displayName</span></span>|<span data-ttu-id="2ef43-137">String</span><span class="sxs-lookup"><span data-stu-id="2ef43-137">String</span></span>|<span data-ttu-id="2ef43-138">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ef43-138">Display name for the device category.</span></span>|
|<span data-ttu-id="2ef43-139">description</span><span class="sxs-lookup"><span data-stu-id="2ef43-139">description</span></span>|<span data-ttu-id="2ef43-140">String</span><span class="sxs-lookup"><span data-stu-id="2ef43-140">String</span></span>|<span data-ttu-id="2ef43-141">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ef43-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="2ef43-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef43-142">Response</span></span>
<span data-ttu-id="2ef43-143">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef43-143">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-onboarding-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ef43-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ef43-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ef43-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef43-145">Request</span></span>
<span data-ttu-id="2ef43-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef43-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2ef43-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef43-147">Response</span></span>
<span data-ttu-id="2ef43-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ef43-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




