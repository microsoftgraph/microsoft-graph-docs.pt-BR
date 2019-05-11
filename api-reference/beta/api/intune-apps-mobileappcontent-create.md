---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d9dcbbc339898eebdf70edabe19b95959fea75c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935311"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="4c1fe-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4c1fe-103">Create mobileAppContent</span></span>

> <span data-ttu-id="4c1fe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c1fe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c1fe-106">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4c1fe-106">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c1fe-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c1fe-107">Prerequisites</span></span>
<span data-ttu-id="4c1fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c1fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c1fe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c1fe-110">Permission type</span></span>|<span data-ttu-id="4c1fe-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c1fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c1fe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c1fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c1fe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1fe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c1fe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c1fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c1fe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-115">Not supported.</span></span>|
|<span data-ttu-id="4c1fe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c1fe-116">Application</span></span>|<span data-ttu-id="4c1fe-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c1fe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c1fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="4c1fe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1fe-119">Request headers</span></span>
|<span data-ttu-id="4c1fe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c1fe-120">Header</span></span>|<span data-ttu-id="4c1fe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c1fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c1fe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c1fe-122">Authorization</span></span>|<span data-ttu-id="4c1fe-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c1fe-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c1fe-124">Accept</span></span>|<span data-ttu-id="4c1fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c1fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c1fe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1fe-126">Request body</span></span>
<span data-ttu-id="4c1fe-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-127">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="4c1fe-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-128">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="4c1fe-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c1fe-129">Property</span></span>|<span data-ttu-id="4c1fe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c1fe-130">Type</span></span>|<span data-ttu-id="4c1fe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c1fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c1fe-132">id</span><span class="sxs-lookup"><span data-stu-id="4c1fe-132">id</span></span>|<span data-ttu-id="4c1fe-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c1fe-133">String</span></span>|<span data-ttu-id="4c1fe-134">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="4c1fe-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c1fe-135">Response</span></span>
<span data-ttu-id="4c1fe-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-136">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c1fe-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c1fe-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c1fe-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1fe-138">Request</span></span>
<span data-ttu-id="4c1fe-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="4c1fe-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c1fe-140">Response</span></span>
<span data-ttu-id="4c1fe-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c1fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




