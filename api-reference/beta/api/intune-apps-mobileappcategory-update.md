---
title: Atualizar mobileAppCategory
description: Atualizar as propriedades de um objeto mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4500d70e3bf86dea2fd58dfe2e0dc387cf97c1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960941"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="ed0e0-103">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="ed0e0-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="ed0e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed0e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed0e0-106">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ed0e0-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed0e0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed0e0-107">Prerequisites</span></span>
<span data-ttu-id="ed0e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed0e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed0e0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed0e0-110">Permission type</span></span>|<span data-ttu-id="ed0e0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed0e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed0e0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed0e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed0e0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed0e0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed0e0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed0e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed0e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-115">Not supported.</span></span>|
|<span data-ttu-id="ed0e0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed0e0-116">Application</span></span>|<span data-ttu-id="ed0e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed0e0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed0e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ed0e0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0e0-119">Request headers</span></span>
|<span data-ttu-id="ed0e0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed0e0-120">Header</span></span>|<span data-ttu-id="ed0e0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed0e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed0e0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed0e0-122">Authorization</span></span>|<span data-ttu-id="ed0e0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed0e0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed0e0-124">Accept</span></span>|<span data-ttu-id="ed0e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed0e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed0e0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0e0-126">Request body</span></span>
<span data-ttu-id="ed0e0-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ed0e0-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="ed0e0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ed0e0-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="ed0e0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed0e0-129">Property</span></span>|<span data-ttu-id="ed0e0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed0e0-130">Type</span></span>|<span data-ttu-id="ed0e0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed0e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed0e0-132">id</span><span class="sxs-lookup"><span data-stu-id="ed0e0-132">id</span></span>|<span data-ttu-id="ed0e0-133">String</span><span class="sxs-lookup"><span data-stu-id="ed0e0-133">String</span></span>|<span data-ttu-id="ed0e0-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-134">The key of the entity.</span></span>|
|<span data-ttu-id="ed0e0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ed0e0-135">displayName</span></span>|<span data-ttu-id="ed0e0-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed0e0-136">String</span></span>|<span data-ttu-id="ed0e0-137">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-137">The name of the app category.</span></span>|
|<span data-ttu-id="ed0e0-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed0e0-138">lastModifiedDateTime</span></span>|<span data-ttu-id="ed0e0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed0e0-139">DateTimeOffset</span></span>|<span data-ttu-id="ed0e0-140">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ed0e0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed0e0-141">Response</span></span>
<span data-ttu-id="ed0e0-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed0e0-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed0e0-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed0e0-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed0e0-144">Request</span></span>
<span data-ttu-id="ed0e0-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ed0e0-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed0e0-146">Response</span></span>
<span data-ttu-id="ed0e0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed0e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





