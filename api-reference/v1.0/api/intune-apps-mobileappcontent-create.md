---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e8debcf1a1b71864465a42635bf1be08033c6659
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358281"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="4246f-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4246f-103">Create mobileAppContent</span></span>

> <span data-ttu-id="4246f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4246f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4246f-105">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4246f-105">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4246f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4246f-106">Prerequisites</span></span>
<span data-ttu-id="4246f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4246f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4246f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4246f-109">Permission type</span></span>|<span data-ttu-id="4246f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4246f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4246f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4246f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4246f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4246f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4246f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4246f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4246f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4246f-114">Not supported.</span></span>|
|<span data-ttu-id="4246f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4246f-115">Application</span></span>|<span data-ttu-id="4246f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4246f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4246f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4246f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="4246f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4246f-118">Request headers</span></span>
|<span data-ttu-id="4246f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4246f-119">Header</span></span>|<span data-ttu-id="4246f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4246f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4246f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4246f-121">Authorization</span></span>|<span data-ttu-id="4246f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4246f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4246f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4246f-123">Accept</span></span>|<span data-ttu-id="4246f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4246f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4246f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4246f-125">Request body</span></span>
<span data-ttu-id="4246f-126">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="4246f-126">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="4246f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="4246f-127">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="4246f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4246f-128">Property</span></span>|<span data-ttu-id="4246f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4246f-129">Type</span></span>|<span data-ttu-id="4246f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4246f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4246f-131">id</span><span class="sxs-lookup"><span data-stu-id="4246f-131">id</span></span>|<span data-ttu-id="4246f-132">String</span><span class="sxs-lookup"><span data-stu-id="4246f-132">String</span></span>|<span data-ttu-id="4246f-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4246f-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="4246f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4246f-134">Response</span></span>
<span data-ttu-id="4246f-135">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4246f-135">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4246f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4246f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4246f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4246f-137">Request</span></span>
<span data-ttu-id="4246f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4246f-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="4246f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4246f-139">Response</span></span>
<span data-ttu-id="4246f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4246f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




