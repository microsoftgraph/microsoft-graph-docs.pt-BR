---
title: Atualizar mobileAppCategory
description: Atualizar as propriedades de um objeto mobileAppCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ebcad7c37c5fc4b6ca94645bef7ebb0a3ccd4763
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515992"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="8cb34-103">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="8cb34-103">Update mobileAppCategory</span></span>

<span data-ttu-id="8cb34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cb34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cb34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cb34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb34-106">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="8cb34-106">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cb34-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cb34-107">Prerequisites</span></span>
<span data-ttu-id="8cb34-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cb34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb34-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cb34-110">Permission type</span></span>|<span data-ttu-id="8cb34-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cb34-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb34-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cb34-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cb34-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb34-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8cb34-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cb34-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb34-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cb34-115">Not supported.</span></span>|
|<span data-ttu-id="8cb34-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cb34-116">Application</span></span>|<span data-ttu-id="8cb34-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cb34-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb34-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cb34-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="8cb34-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb34-119">Request headers</span></span>
|<span data-ttu-id="8cb34-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cb34-120">Header</span></span>|<span data-ttu-id="8cb34-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8cb34-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb34-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cb34-122">Authorization</span></span>|<span data-ttu-id="8cb34-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cb34-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb34-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cb34-124">Accept</span></span>|<span data-ttu-id="8cb34-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb34-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb34-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb34-126">Request body</span></span>
<span data-ttu-id="8cb34-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="8cb34-127">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="8cb34-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="8cb34-128">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="8cb34-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cb34-129">Property</span></span>|<span data-ttu-id="8cb34-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cb34-130">Type</span></span>|<span data-ttu-id="8cb34-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cb34-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb34-132">id</span><span class="sxs-lookup"><span data-stu-id="8cb34-132">id</span></span>|<span data-ttu-id="8cb34-133">String</span><span class="sxs-lookup"><span data-stu-id="8cb34-133">String</span></span>|<span data-ttu-id="8cb34-134">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8cb34-134">The key of the entity.</span></span>|
|<span data-ttu-id="8cb34-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8cb34-135">displayName</span></span>|<span data-ttu-id="8cb34-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cb34-136">String</span></span>|<span data-ttu-id="8cb34-137">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cb34-137">The name of the app category.</span></span>|
|<span data-ttu-id="8cb34-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb34-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8cb34-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb34-139">DateTimeOffset</span></span>|<span data-ttu-id="8cb34-140">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8cb34-140">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8cb34-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb34-141">Response</span></span>
<span data-ttu-id="8cb34-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cb34-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb34-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cb34-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cb34-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cb34-144">Request</span></span>
<span data-ttu-id="8cb34-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cb34-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="8cb34-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cb34-146">Response</span></span>
<span data-ttu-id="8cb34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cb34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




