---
title: Atualizar mobileAppCategory
description: Atualizar as propriedades de um objeto mobileAppCategory.
author: tfitzmac
ms.openlocfilehash: ac7bc0d0efab32f659e3e171a2585af8ff992ea1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346316"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="81f3b-103">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="81f3b-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="81f3b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="81f3b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81f3b-105">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="81f3b-105">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81f3b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81f3b-106">Prerequisites</span></span>
<span data-ttu-id="81f3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81f3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81f3b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81f3b-109">Permission type</span></span>|<span data-ttu-id="81f3b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81f3b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81f3b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81f3b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81f3b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f3b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81f3b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81f3b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81f3b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81f3b-114">Not supported.</span></span>|
|<span data-ttu-id="81f3b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81f3b-115">Application</span></span>|<span data-ttu-id="81f3b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81f3b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81f3b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81f3b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="81f3b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81f3b-118">Request headers</span></span>
|<span data-ttu-id="81f3b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81f3b-119">Header</span></span>|<span data-ttu-id="81f3b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="81f3b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81f3b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="81f3b-121">Authorization</span></span>|<span data-ttu-id="81f3b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81f3b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81f3b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="81f3b-123">Accept</span></span>|<span data-ttu-id="81f3b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="81f3b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81f3b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81f3b-125">Request body</span></span>
<span data-ttu-id="81f3b-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="81f3b-126">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="81f3b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="81f3b-127">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="81f3b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81f3b-128">Property</span></span>|<span data-ttu-id="81f3b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f3b-129">Type</span></span>|<span data-ttu-id="81f3b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f3b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f3b-131">id</span><span class="sxs-lookup"><span data-stu-id="81f3b-131">id</span></span>|<span data-ttu-id="81f3b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f3b-132">String</span></span>|<span data-ttu-id="81f3b-133">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="81f3b-133">The key of the entity.</span></span>|
|<span data-ttu-id="81f3b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="81f3b-134">displayName</span></span>|<span data-ttu-id="81f3b-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81f3b-135">String</span></span>|<span data-ttu-id="81f3b-136">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="81f3b-136">The name of the app category.</span></span>|
|<span data-ttu-id="81f3b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81f3b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="81f3b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81f3b-138">DateTimeOffset</span></span>|<span data-ttu-id="81f3b-139">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="81f3b-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="81f3b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="81f3b-140">Response</span></span>
<span data-ttu-id="81f3b-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81f3b-141">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81f3b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81f3b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="81f3b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81f3b-143">Request</span></span>
<span data-ttu-id="81f3b-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81f3b-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="81f3b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="81f3b-145">Response</span></span>
<span data-ttu-id="81f3b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81f3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



