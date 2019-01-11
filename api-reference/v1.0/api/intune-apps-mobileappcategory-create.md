---
title: Criar mobileAppCategory
description: Criar um novo objeto mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c09b557da645767e090bfecca7974c0af41b17f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870795"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="baa26-103">Criar mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="baa26-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="baa26-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="baa26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baa26-105">Criar um novo objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="baa26-105">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baa26-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="baa26-106">Prerequisites</span></span>
<span data-ttu-id="baa26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baa26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baa26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="baa26-109">Permission type</span></span>|<span data-ttu-id="baa26-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="baa26-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baa26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="baa26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="baa26-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa26-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="baa26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="baa26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baa26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baa26-114">Not supported.</span></span>|
|<span data-ttu-id="baa26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="baa26-115">Application</span></span>|<span data-ttu-id="baa26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="baa26-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baa26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="baa26-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="baa26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="baa26-118">Request headers</span></span>
|<span data-ttu-id="baa26-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="baa26-119">Header</span></span>|<span data-ttu-id="baa26-120">Valor</span><span class="sxs-lookup"><span data-stu-id="baa26-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baa26-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="baa26-121">Authorization</span></span>|<span data-ttu-id="baa26-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="baa26-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baa26-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="baa26-123">Accept</span></span>|<span data-ttu-id="baa26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="baa26-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baa26-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="baa26-125">Request body</span></span>
<span data-ttu-id="baa26-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="baa26-126">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="baa26-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="baa26-127">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="baa26-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="baa26-128">Property</span></span>|<span data-ttu-id="baa26-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="baa26-129">Type</span></span>|<span data-ttu-id="baa26-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="baa26-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa26-131">id</span><span class="sxs-lookup"><span data-stu-id="baa26-131">id</span></span>|<span data-ttu-id="baa26-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="baa26-132">String</span></span>|<span data-ttu-id="baa26-133">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="baa26-133">The key of the entity.</span></span>|
|<span data-ttu-id="baa26-134">displayName</span><span class="sxs-lookup"><span data-stu-id="baa26-134">displayName</span></span>|<span data-ttu-id="baa26-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="baa26-135">String</span></span>|<span data-ttu-id="baa26-136">O nome da categoria do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="baa26-136">The name of the app category.</span></span>|
|<span data-ttu-id="baa26-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baa26-137">lastModifiedDateTime</span></span>|<span data-ttu-id="baa26-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baa26-138">DateTimeOffset</span></span>|<span data-ttu-id="baa26-139">A data e hora que a mobileAppCategory foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="baa26-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="baa26-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="baa26-140">Response</span></span>
<span data-ttu-id="baa26-141">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="baa26-141">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baa26-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="baa26-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="baa26-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="baa26-143">Request</span></span>
<span data-ttu-id="baa26-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="baa26-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="baa26-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="baa26-145">Response</span></span>
<span data-ttu-id="baa26-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="baa26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



