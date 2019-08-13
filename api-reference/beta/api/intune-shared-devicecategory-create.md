---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9100345393126bb699236a42309715a1e1f94102
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350948"
---
# <a name="create-devicecategory"></a><span data-ttu-id="db1a6-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="db1a6-103">Create deviceCategory</span></span>

> <span data-ttu-id="db1a6-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db1a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="db1a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db1a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db1a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db1a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db1a6-107">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="db1a6-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db1a6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db1a6-108">Prerequisites</span></span>

<span data-ttu-id="db1a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db1a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db1a6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db1a6-111">Permission type</span></span>|<span data-ttu-id="db1a6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db1a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db1a6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db1a6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="db1a6-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="db1a6-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="db1a6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db1a6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="db1a6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db1a6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db1a6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db1a6-117">Not supported.</span></span>|
|<span data-ttu-id="db1a6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db1a6-118">Application</span></span>|<span data-ttu-id="db1a6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db1a6-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db1a6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db1a6-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="db1a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db1a6-121">Request headers</span></span>

|<span data-ttu-id="db1a6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db1a6-122">Header</span></span>|<span data-ttu-id="db1a6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="db1a6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db1a6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="db1a6-124">Authorization</span></span>|<span data-ttu-id="db1a6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db1a6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db1a6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db1a6-126">Accept</span></span>|<span data-ttu-id="db1a6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="db1a6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db1a6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db1a6-128">Request body</span></span>

<span data-ttu-id="db1a6-129">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="db1a6-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="db1a6-130">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="db1a6-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="db1a6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db1a6-131">Property</span></span>|<span data-ttu-id="db1a6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="db1a6-132">Type</span></span>|<span data-ttu-id="db1a6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="db1a6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db1a6-134">id</span><span class="sxs-lookup"><span data-stu-id="db1a6-134">id</span></span>|<span data-ttu-id="db1a6-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db1a6-135">String</span></span>|<span data-ttu-id="db1a6-136">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db1a6-136">Unique identifier for the device category.</span></span> <span data-ttu-id="db1a6-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db1a6-137">Read-only.</span></span>|
|<span data-ttu-id="db1a6-138">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="db1a6-138">**Obboarding**</span></span>|
|<span data-ttu-id="db1a6-139">descrição</span><span class="sxs-lookup"><span data-stu-id="db1a6-139">description</span></span>|<span data-ttu-id="db1a6-140">String</span><span class="sxs-lookup"><span data-stu-id="db1a6-140">String</span></span>|<span data-ttu-id="db1a6-141">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db1a6-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="db1a6-142">displayName</span><span class="sxs-lookup"><span data-stu-id="db1a6-142">displayName</span></span>|<span data-ttu-id="db1a6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db1a6-143">String</span></span>|<span data-ttu-id="db1a6-144">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db1a6-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="db1a6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="db1a6-145">Response</span></span>

<span data-ttu-id="db1a6-146">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db1a6-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db1a6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db1a6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="db1a6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db1a6-148">Request</span></span>

<span data-ttu-id="db1a6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db1a6-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="db1a6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="db1a6-150">Response</span></span>

<span data-ttu-id="db1a6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db1a6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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






