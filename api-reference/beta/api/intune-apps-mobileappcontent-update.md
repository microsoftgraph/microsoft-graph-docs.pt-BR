---
title: Atualizar mobileAppContent
description: Atualizar as propriedades de um objeto mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a5ee651cc363756a4d9508eb4c772ee530b16ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43415631"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="cfdb4-103">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="cfdb4-103">Update mobileAppContent</span></span>

<span data-ttu-id="cfdb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfdb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfdb4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfdb4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfdb4-107">Atualizar as propriedades de um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cfdb4-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfdb4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfdb4-108">Prerequisites</span></span>
<span data-ttu-id="cfdb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfdb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfdb4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfdb4-111">Permission type</span></span>|<span data-ttu-id="cfdb4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfdb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfdb4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfdb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfdb4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdb4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cfdb4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfdb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfdb4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-116">Not supported.</span></span>|
|<span data-ttu-id="cfdb4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfdb4-117">Application</span></span>|<span data-ttu-id="cfdb4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfdb4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfdb4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfdb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="cfdb4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdb4-120">Request headers</span></span>
|<span data-ttu-id="cfdb4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfdb4-121">Header</span></span>|<span data-ttu-id="cfdb4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cfdb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfdb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfdb4-123">Authorization</span></span>|<span data-ttu-id="cfdb4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfdb4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfdb4-125">Accept</span></span>|<span data-ttu-id="cfdb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfdb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfdb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdb4-127">Request body</span></span>
<span data-ttu-id="cfdb4-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cfdb4-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="cfdb4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="cfdb4-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="cfdb4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfdb4-130">Property</span></span>|<span data-ttu-id="cfdb4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfdb4-131">Type</span></span>|<span data-ttu-id="cfdb4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfdb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfdb4-133">id</span><span class="sxs-lookup"><span data-stu-id="cfdb4-133">id</span></span>|<span data-ttu-id="cfdb4-134">String</span><span class="sxs-lookup"><span data-stu-id="cfdb4-134">String</span></span>|<span data-ttu-id="cfdb4-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="cfdb4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdb4-136">Response</span></span>
<span data-ttu-id="cfdb4-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfdb4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfdb4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfdb4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfdb4-139">Request</span></span>
<span data-ttu-id="cfdb4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="cfdb4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfdb4-141">Response</span></span>
<span data-ttu-id="cfdb4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfdb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



