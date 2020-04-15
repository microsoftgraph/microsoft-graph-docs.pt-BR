---
title: Atualizar mobileAppContent
description: Atualizar as propriedades de um objeto mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05febed512ef2ecc8d0e03bab02c432d1f3d0fa5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464749"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="089d3-103">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="089d3-103">Update mobileAppContent</span></span>

<span data-ttu-id="089d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="089d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="089d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="089d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089d3-106">Atualizar as propriedades de um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="089d3-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="089d3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="089d3-107">Prerequisites</span></span>
<span data-ttu-id="089d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="089d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="089d3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="089d3-110">Permission type</span></span>|<span data-ttu-id="089d3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="089d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="089d3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="089d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="089d3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="089d3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="089d3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="089d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="089d3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="089d3-115">Not supported.</span></span>|
|<span data-ttu-id="089d3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="089d3-116">Application</span></span>|<span data-ttu-id="089d3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="089d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="089d3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="089d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="089d3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="089d3-119">Request headers</span></span>
|<span data-ttu-id="089d3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="089d3-120">Header</span></span>|<span data-ttu-id="089d3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="089d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="089d3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="089d3-122">Authorization</span></span>|<span data-ttu-id="089d3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="089d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="089d3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="089d3-124">Accept</span></span>|<span data-ttu-id="089d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="089d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="089d3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="089d3-126">Request body</span></span>
<span data-ttu-id="089d3-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="089d3-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="089d3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="089d3-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="089d3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="089d3-129">Property</span></span>|<span data-ttu-id="089d3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="089d3-130">Type</span></span>|<span data-ttu-id="089d3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="089d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089d3-132">id</span><span class="sxs-lookup"><span data-stu-id="089d3-132">id</span></span>|<span data-ttu-id="089d3-133">String</span><span class="sxs-lookup"><span data-stu-id="089d3-133">String</span></span>|<span data-ttu-id="089d3-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="089d3-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="089d3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="089d3-135">Response</span></span>
<span data-ttu-id="089d3-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="089d3-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="089d3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="089d3-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="089d3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="089d3-138">Request</span></span>
<span data-ttu-id="089d3-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="089d3-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="089d3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="089d3-140">Response</span></span>
<span data-ttu-id="089d3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="089d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```






