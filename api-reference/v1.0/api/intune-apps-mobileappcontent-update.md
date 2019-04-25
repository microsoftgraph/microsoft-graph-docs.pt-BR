---
title: Atualizar mobileAppContent
description: Atualizar as propriedades de um objeto mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c2a3a1003ef2cd948778c84dc8dd8f204994ee1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541623"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="854df-103">Atualizar mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="854df-103">Update mobileAppContent</span></span>

> <span data-ttu-id="854df-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="854df-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="854df-105">Atualizar as propriedades de um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="854df-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="854df-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="854df-106">Prerequisites</span></span>
<span data-ttu-id="854df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="854df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="854df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="854df-109">Permission type</span></span>|<span data-ttu-id="854df-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="854df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="854df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="854df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="854df-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="854df-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="854df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="854df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="854df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="854df-114">Not supported.</span></span>|
|<span data-ttu-id="854df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="854df-115">Application</span></span>|<span data-ttu-id="854df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="854df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="854df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="854df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="854df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="854df-118">Request headers</span></span>
|<span data-ttu-id="854df-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="854df-119">Header</span></span>|<span data-ttu-id="854df-120">Valor</span><span class="sxs-lookup"><span data-stu-id="854df-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="854df-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="854df-121">Authorization</span></span>|<span data-ttu-id="854df-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="854df-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="854df-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="854df-123">Accept</span></span>|<span data-ttu-id="854df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="854df-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="854df-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="854df-125">Request body</span></span>
<span data-ttu-id="854df-126">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="854df-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="854df-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="854df-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="854df-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="854df-128">Property</span></span>|<span data-ttu-id="854df-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="854df-129">Type</span></span>|<span data-ttu-id="854df-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="854df-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="854df-131">id</span><span class="sxs-lookup"><span data-stu-id="854df-131">id</span></span>|<span data-ttu-id="854df-132">String</span><span class="sxs-lookup"><span data-stu-id="854df-132">String</span></span>|<span data-ttu-id="854df-133">A versão do conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="854df-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="854df-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="854df-134">Response</span></span>
<span data-ttu-id="854df-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [mobileAppContent](../resources/intune-apps-mobileappcontent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="854df-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="854df-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="854df-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="854df-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="854df-137">Request</span></span>
<span data-ttu-id="854df-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="854df-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="854df-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="854df-139">Response</span></span>
<span data-ttu-id="854df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="854df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



