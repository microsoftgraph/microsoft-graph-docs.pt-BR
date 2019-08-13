---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a50b4c3cd7e236bf5fdc2cc3a1d18e75fb7e526d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329261"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="7e08c-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="7e08c-103">Create mobileAppContent</span></span>

> <span data-ttu-id="7e08c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e08c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e08c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e08c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e08c-106">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="7e08c-106">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e08c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e08c-107">Prerequisites</span></span>
<span data-ttu-id="7e08c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e08c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e08c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e08c-110">Permission type</span></span>|<span data-ttu-id="7e08c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e08c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e08c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e08c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e08c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e08c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e08c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e08c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e08c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e08c-115">Not supported.</span></span>|
|<span data-ttu-id="7e08c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e08c-116">Application</span></span>|<span data-ttu-id="7e08c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e08c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e08c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e08c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="7e08c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e08c-119">Request headers</span></span>
|<span data-ttu-id="7e08c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e08c-120">Header</span></span>|<span data-ttu-id="7e08c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7e08c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e08c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e08c-122">Authorization</span></span>|<span data-ttu-id="7e08c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e08c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e08c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e08c-124">Accept</span></span>|<span data-ttu-id="7e08c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e08c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e08c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e08c-126">Request body</span></span>
<span data-ttu-id="7e08c-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="7e08c-127">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="7e08c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="7e08c-128">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="7e08c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e08c-129">Property</span></span>|<span data-ttu-id="7e08c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e08c-130">Type</span></span>|<span data-ttu-id="7e08c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e08c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e08c-132">id</span><span class="sxs-lookup"><span data-stu-id="7e08c-132">id</span></span>|<span data-ttu-id="7e08c-133">String</span><span class="sxs-lookup"><span data-stu-id="7e08c-133">String</span></span>|<span data-ttu-id="7e08c-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7e08c-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="7e08c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e08c-135">Response</span></span>
<span data-ttu-id="7e08c-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e08c-136">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e08c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e08c-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e08c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e08c-138">Request</span></span>
<span data-ttu-id="7e08c-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e08c-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="7e08c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e08c-140">Response</span></span>
<span data-ttu-id="7e08c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e08c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```






