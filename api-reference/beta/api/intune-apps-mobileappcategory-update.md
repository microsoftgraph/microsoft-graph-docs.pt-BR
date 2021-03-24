---
title: Atualizar mobileAppCategory
description: Atualizar as propriedades de um objeto mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d19dcdb6c4223df10b657d2e599d7803878a82c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143294"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="eeb92-103">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="eeb92-103">Update mobileAppCategory</span></span>

<span data-ttu-id="eeb92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeb92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eeb92-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eeb92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeb92-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eeb92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeb92-107">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="eeb92-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eeb92-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eeb92-108">Prerequisites</span></span>
<span data-ttu-id="eeb92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeb92-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eeb92-111">Permission type</span></span>|<span data-ttu-id="eeb92-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eeb92-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeb92-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eeb92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eeb92-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeb92-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eeb92-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eeb92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeb92-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eeb92-116">Not supported.</span></span>|
|<span data-ttu-id="eeb92-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eeb92-117">Application</span></span>|<span data-ttu-id="eeb92-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeb92-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeb92-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eeb92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="eeb92-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb92-120">Request headers</span></span>
|<span data-ttu-id="eeb92-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eeb92-121">Header</span></span>|<span data-ttu-id="eeb92-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eeb92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeb92-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eeb92-123">Authorization</span></span>|<span data-ttu-id="eeb92-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eeb92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeb92-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eeb92-125">Accept</span></span>|<span data-ttu-id="eeb92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eeb92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeb92-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb92-127">Request body</span></span>
<span data-ttu-id="eeb92-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="eeb92-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="eeb92-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="eeb92-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="eeb92-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb92-130">Property</span></span>|<span data-ttu-id="eeb92-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb92-131">Type</span></span>|<span data-ttu-id="eeb92-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeb92-133">id</span><span class="sxs-lookup"><span data-stu-id="eeb92-133">id</span></span>|<span data-ttu-id="eeb92-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb92-134">String</span></span>|<span data-ttu-id="eeb92-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eeb92-135">The key of the entity.</span></span>|
|<span data-ttu-id="eeb92-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eeb92-136">displayName</span></span>|<span data-ttu-id="eeb92-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb92-137">String</span></span>|<span data-ttu-id="eeb92-138">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eeb92-138">The name of the app category.</span></span>|
|<span data-ttu-id="eeb92-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eeb92-139">lastModifiedDateTime</span></span>|<span data-ttu-id="eeb92-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeb92-140">DateTimeOffset</span></span>|<span data-ttu-id="eeb92-141">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="eeb92-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="eeb92-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeb92-142">Response</span></span>
<span data-ttu-id="eeb92-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eeb92-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeb92-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eeb92-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="eeb92-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb92-145">Request</span></span>
<span data-ttu-id="eeb92-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eeb92-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="eeb92-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeb92-147">Response</span></span>
<span data-ttu-id="eeb92-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eeb92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




