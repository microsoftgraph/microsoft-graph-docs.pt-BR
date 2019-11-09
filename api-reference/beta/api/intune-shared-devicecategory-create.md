---
title: Criar deviceCategory
description: Cria um novo objeto deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b41a7a98bb5a9f7f42215fd127914246c132784
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086239"
---
# <a name="create-devicecategory"></a><span data-ttu-id="36147-103">Criar deviceCategory</span><span class="sxs-lookup"><span data-stu-id="36147-103">Create deviceCategory</span></span>

> <span data-ttu-id="36147-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="36147-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="36147-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36147-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36147-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36147-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36147-107">Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="36147-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36147-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36147-108">Prerequisites</span></span>

<span data-ttu-id="36147-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36147-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36147-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36147-111">Permission type</span></span>|<span data-ttu-id="36147-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36147-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36147-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36147-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="36147-114">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="36147-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="36147-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36147-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="36147-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36147-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36147-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36147-117">Not supported.</span></span>|
|<span data-ttu-id="36147-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36147-118">Application</span></span>||
| <span data-ttu-id="36147-119">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="36147-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="36147-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36147-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36147-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36147-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="36147-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36147-122">Request headers</span></span>

|<span data-ttu-id="36147-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36147-123">Header</span></span>|<span data-ttu-id="36147-124">Valor</span><span class="sxs-lookup"><span data-stu-id="36147-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36147-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="36147-125">Authorization</span></span>|<span data-ttu-id="36147-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36147-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36147-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36147-127">Accept</span></span>|<span data-ttu-id="36147-128">application/json</span><span class="sxs-lookup"><span data-stu-id="36147-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36147-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36147-129">Request body</span></span>

<span data-ttu-id="36147-130">No corpo da solicitação, forneça uma representação JSON do objeto deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="36147-130">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="36147-131">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="36147-131">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="36147-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36147-132">Property</span></span>|<span data-ttu-id="36147-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="36147-133">Type</span></span>|<span data-ttu-id="36147-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="36147-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36147-135">id</span><span class="sxs-lookup"><span data-stu-id="36147-135">id</span></span>|<span data-ttu-id="36147-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36147-136">String</span></span>|<span data-ttu-id="36147-137">O identificador exclusivo da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36147-137">Unique identifier for the device category.</span></span> <span data-ttu-id="36147-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36147-138">Read-only.</span></span>|
|<span data-ttu-id="36147-139">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="36147-139">**Obboarding**</span></span>|
|<span data-ttu-id="36147-140">descrição</span><span class="sxs-lookup"><span data-stu-id="36147-140">description</span></span>|<span data-ttu-id="36147-141">String</span><span class="sxs-lookup"><span data-stu-id="36147-141">String</span></span>|<span data-ttu-id="36147-142">Descrição opcional da categoria do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36147-142">Optional description for the device category.</span></span>|
|<span data-ttu-id="36147-143">displayName</span><span class="sxs-lookup"><span data-stu-id="36147-143">displayName</span></span>|<span data-ttu-id="36147-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36147-144">String</span></span>|<span data-ttu-id="36147-145">Nome de exibição da categoria de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36147-145">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="36147-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="36147-146">Response</span></span>

<span data-ttu-id="36147-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCategory](../resources/intune-shared-devicecategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36147-147">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36147-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36147-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="36147-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36147-149">Request</span></span>

<span data-ttu-id="36147-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36147-150">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="36147-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="36147-151">Response</span></span>

<span data-ttu-id="36147-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36147-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












