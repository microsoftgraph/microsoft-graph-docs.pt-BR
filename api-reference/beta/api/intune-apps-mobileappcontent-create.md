---
title: Criar mobileAppContent
description: Criar um novo objeto mobileAppContent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11e86c77e1c6e8359756c924c10d1626b565d00c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445019"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="874fd-103">Criar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="874fd-103">Create mobileAppContent</span></span>

<span data-ttu-id="874fd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="874fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="874fd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="874fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="874fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="874fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="874fd-107">Criar um novo objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="874fd-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="874fd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="874fd-108">Prerequisites</span></span>
<span data-ttu-id="874fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874fd-111">Permission type</span></span>|<span data-ttu-id="874fd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="874fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="874fd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="874fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="874fd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="874fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="874fd-116">Not supported.</span></span>|
|<span data-ttu-id="874fd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="874fd-117">Application</span></span>|<span data-ttu-id="874fd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874fd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="874fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="874fd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874fd-120">Request headers</span></span>
|<span data-ttu-id="874fd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="874fd-121">Header</span></span>|<span data-ttu-id="874fd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="874fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="874fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="874fd-123">Authorization</span></span>|<span data-ttu-id="874fd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="874fd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="874fd-125">Accept</span></span>|<span data-ttu-id="874fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="874fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="874fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874fd-127">Request body</span></span>
<span data-ttu-id="874fd-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="874fd-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="874fd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="874fd-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="874fd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="874fd-130">Property</span></span>|<span data-ttu-id="874fd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="874fd-131">Type</span></span>|<span data-ttu-id="874fd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="874fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="874fd-133">id</span><span class="sxs-lookup"><span data-stu-id="874fd-133">id</span></span>|<span data-ttu-id="874fd-134">String</span><span class="sxs-lookup"><span data-stu-id="874fd-134">String</span></span>|<span data-ttu-id="874fd-135">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="874fd-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="874fd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="874fd-136">Response</span></span>
<span data-ttu-id="874fd-137">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874fd-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="874fd-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="874fd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="874fd-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874fd-139">Request</span></span>
<span data-ttu-id="874fd-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874fd-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="874fd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="874fd-141">Response</span></span>
<span data-ttu-id="874fd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="874fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





