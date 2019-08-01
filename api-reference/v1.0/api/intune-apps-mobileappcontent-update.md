---
title: Atualizar mobileAppContent
description: Atualizar as propriedades de um objeto mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2718dd551a1d9bf1d5210d3d668e0bd26951c6fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002024"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="fbaa7-103">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="fbaa7-103">Update mobileAppContent</span></span>

> <span data-ttu-id="fbaa7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbaa7-105">Atualizar as propriedades de um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="fbaa7-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbaa7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbaa7-106">Prerequisites</span></span>
<span data-ttu-id="fbaa7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbaa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbaa7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbaa7-109">Permission type</span></span>|<span data-ttu-id="fbaa7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbaa7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbaa7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbaa7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbaa7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbaa7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbaa7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbaa7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbaa7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-114">Not supported.</span></span>|
|<span data-ttu-id="fbaa7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbaa7-115">Application</span></span>|<span data-ttu-id="fbaa7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbaa7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbaa7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="fbaa7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaa7-118">Request headers</span></span>
|<span data-ttu-id="fbaa7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbaa7-119">Header</span></span>|<span data-ttu-id="fbaa7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fbaa7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbaa7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbaa7-121">Authorization</span></span>|<span data-ttu-id="fbaa7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbaa7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbaa7-123">Accept</span></span>|<span data-ttu-id="fbaa7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fbaa7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbaa7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaa7-125">Request body</span></span>
<span data-ttu-id="fbaa7-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="fbaa7-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="fbaa7-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="fbaa7-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="fbaa7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbaa7-128">Property</span></span>|<span data-ttu-id="fbaa7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbaa7-129">Type</span></span>|<span data-ttu-id="fbaa7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbaa7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbaa7-131">id</span><span class="sxs-lookup"><span data-stu-id="fbaa7-131">id</span></span>|<span data-ttu-id="fbaa7-132">String</span><span class="sxs-lookup"><span data-stu-id="fbaa7-132">String</span></span>|<span data-ttu-id="fbaa7-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="fbaa7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbaa7-134">Response</span></span>
<span data-ttu-id="fbaa7-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbaa7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbaa7-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbaa7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaa7-137">Request</span></span>
<span data-ttu-id="fbaa7-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="fbaa7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbaa7-139">Response</span></span>
<span data-ttu-id="fbaa7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbaa7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



