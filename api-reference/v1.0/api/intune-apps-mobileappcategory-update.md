---
title: Atualizar mobileAppCategory
description: Atualizar as propriedades de um objeto mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e20f15e17df63ec706880922fedb6b1c80e646a4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252543"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="fcf1b-103">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="fcf1b-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="fcf1b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcf1b-105">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="fcf1b-105">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcf1b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fcf1b-106">Prerequisites</span></span>
<span data-ttu-id="fcf1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcf1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fcf1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fcf1b-109">Permission type</span></span>|<span data-ttu-id="fcf1b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fcf1b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcf1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fcf1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fcf1b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf1b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcf1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fcf1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcf1b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-114">Not supported.</span></span>|
|<span data-ttu-id="fcf1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fcf1b-115">Application</span></span>|<span data-ttu-id="fcf1b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcf1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fcf1b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="fcf1b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf1b-118">Request headers</span></span>
|<span data-ttu-id="fcf1b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fcf1b-119">Header</span></span>|<span data-ttu-id="fcf1b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fcf1b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcf1b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fcf1b-121">Authorization</span></span>|<span data-ttu-id="fcf1b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcf1b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fcf1b-123">Accept</span></span>|<span data-ttu-id="fcf1b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fcf1b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcf1b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf1b-125">Request body</span></span>
<span data-ttu-id="fcf1b-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="fcf1b-126">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="fcf1b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="fcf1b-127">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="fcf1b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcf1b-128">Property</span></span>|<span data-ttu-id="fcf1b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcf1b-129">Type</span></span>|<span data-ttu-id="fcf1b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcf1b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcf1b-131">id</span><span class="sxs-lookup"><span data-stu-id="fcf1b-131">id</span></span>|<span data-ttu-id="fcf1b-132">String</span><span class="sxs-lookup"><span data-stu-id="fcf1b-132">String</span></span>|<span data-ttu-id="fcf1b-133">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-133">The key of the entity.</span></span>|
|<span data-ttu-id="fcf1b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fcf1b-134">displayName</span></span>|<span data-ttu-id="fcf1b-135">String</span><span class="sxs-lookup"><span data-stu-id="fcf1b-135">String</span></span>|<span data-ttu-id="fcf1b-136">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-136">The name of the app category.</span></span>|
|<span data-ttu-id="fcf1b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcf1b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fcf1b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcf1b-138">DateTimeOffset</span></span>|<span data-ttu-id="fcf1b-139">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="fcf1b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf1b-140">Response</span></span>
<span data-ttu-id="fcf1b-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-141">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcf1b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fcf1b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcf1b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fcf1b-143">Request</span></span>
<span data-ttu-id="fcf1b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="fcf1b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fcf1b-145">Response</span></span>
<span data-ttu-id="fcf1b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fcf1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



