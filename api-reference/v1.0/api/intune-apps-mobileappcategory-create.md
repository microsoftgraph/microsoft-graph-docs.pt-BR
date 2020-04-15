---
title: Criar mobileAppCategory
description: Criar um novo objeto mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7894965d771e1d92c4b8fbfe81dd65cb4dbf1aae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464869"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="68261-103">Criar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="68261-103">Create mobileAppCategory</span></span>

<span data-ttu-id="68261-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68261-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68261-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68261-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68261-106">Criar um novo objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="68261-106">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68261-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="68261-107">Prerequisites</span></span>
<span data-ttu-id="68261-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68261-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68261-110">Permission type</span></span>|<span data-ttu-id="68261-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="68261-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68261-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68261-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68261-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68261-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68261-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68261-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68261-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68261-115">Not supported.</span></span>|
|<span data-ttu-id="68261-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68261-116">Application</span></span>|<span data-ttu-id="68261-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68261-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68261-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68261-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="68261-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68261-119">Request headers</span></span>
|<span data-ttu-id="68261-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="68261-120">Header</span></span>|<span data-ttu-id="68261-121">Valor</span><span class="sxs-lookup"><span data-stu-id="68261-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68261-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="68261-122">Authorization</span></span>|<span data-ttu-id="68261-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68261-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68261-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="68261-124">Accept</span></span>|<span data-ttu-id="68261-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68261-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68261-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68261-126">Request body</span></span>
<span data-ttu-id="68261-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="68261-127">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="68261-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="68261-128">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="68261-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68261-129">Property</span></span>|<span data-ttu-id="68261-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="68261-130">Type</span></span>|<span data-ttu-id="68261-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="68261-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68261-132">id</span><span class="sxs-lookup"><span data-stu-id="68261-132">id</span></span>|<span data-ttu-id="68261-133">String</span><span class="sxs-lookup"><span data-stu-id="68261-133">String</span></span>|<span data-ttu-id="68261-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="68261-134">The key of the entity.</span></span>|
|<span data-ttu-id="68261-135">displayName</span><span class="sxs-lookup"><span data-stu-id="68261-135">displayName</span></span>|<span data-ttu-id="68261-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68261-136">String</span></span>|<span data-ttu-id="68261-137">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68261-137">The name of the app category.</span></span>|
|<span data-ttu-id="68261-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68261-138">lastModifiedDateTime</span></span>|<span data-ttu-id="68261-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68261-139">DateTimeOffset</span></span>|<span data-ttu-id="68261-140">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="68261-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="68261-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="68261-141">Response</span></span>
<span data-ttu-id="68261-142">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68261-142">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68261-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68261-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="68261-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68261-144">Request</span></span>
<span data-ttu-id="68261-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68261-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="68261-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="68261-146">Response</span></span>
<span data-ttu-id="68261-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68261-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






