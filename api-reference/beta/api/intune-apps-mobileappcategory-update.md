---
title: Atualizar mobileAppCategory
description: Atualizar as propriedades de um objeto mobileAppCategory.
author: tfitzmac
ms.openlocfilehash: c7c53344d28dc60dc5c0dc306615a3d700cdcf82
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325813"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="ef868-103">Atualizar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="ef868-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="ef868-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ef868-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef868-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ef868-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef868-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ef868-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef868-107">Atualizar as propriedades de um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ef868-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef868-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef868-108">Prerequisites</span></span>
<span data-ttu-id="ef868-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef868-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef868-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef868-111">Permission type</span></span>|<span data-ttu-id="ef868-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef868-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef868-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef868-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef868-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef868-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef868-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef868-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef868-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef868-116">Not supported.</span></span>|
|<span data-ttu-id="ef868-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef868-117">Application</span></span>|<span data-ttu-id="ef868-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef868-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef868-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef868-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ef868-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef868-120">Request headers</span></span>
|<span data-ttu-id="ef868-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef868-121">Header</span></span>|<span data-ttu-id="ef868-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef868-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef868-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef868-123">Authorization</span></span>|<span data-ttu-id="ef868-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef868-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef868-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef868-125">Accept</span></span>|<span data-ttu-id="ef868-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef868-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef868-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef868-127">Request body</span></span>
<span data-ttu-id="ef868-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ef868-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="ef868-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="ef868-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="ef868-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef868-130">Property</span></span>|<span data-ttu-id="ef868-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef868-131">Type</span></span>|<span data-ttu-id="ef868-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef868-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef868-133">id</span><span class="sxs-lookup"><span data-stu-id="ef868-133">id</span></span>|<span data-ttu-id="ef868-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef868-134">String</span></span>|<span data-ttu-id="ef868-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef868-135">The key of the entity.</span></span>|
|<span data-ttu-id="ef868-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ef868-136">displayName</span></span>|<span data-ttu-id="ef868-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef868-137">String</span></span>|<span data-ttu-id="ef868-138">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ef868-138">The name of the app category.</span></span>|
|<span data-ttu-id="ef868-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef868-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ef868-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef868-140">DateTimeOffset</span></span>|<span data-ttu-id="ef868-141">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ef868-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ef868-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef868-142">Response</span></span>
<span data-ttu-id="ef868-143">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef868-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef868-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef868-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef868-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef868-145">Request</span></span>
<span data-ttu-id="ef868-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef868-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ef868-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef868-147">Response</span></span>
<span data-ttu-id="ef868-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef868-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





