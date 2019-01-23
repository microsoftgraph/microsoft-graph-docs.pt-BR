---
title: Listar mobileAppContents
description: Listar propriedades e relações dos objetos mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa8cb4e7fbe5cb8e76d8fe2c698678d498c81a6a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397719"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="c8730-103">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="c8730-103">List mobileAppContents</span></span>

> <span data-ttu-id="c8730-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8730-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8730-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8730-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8730-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c8730-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8730-107">Listar propriedades e relações dos objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c8730-107">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8730-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c8730-108">Prerequisites</span></span>
<span data-ttu-id="c8730-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8730-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8730-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c8730-111">Permission type</span></span>|<span data-ttu-id="c8730-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c8730-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8730-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c8730-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8730-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8730-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8730-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c8730-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8730-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8730-116">Not supported.</span></span>|
|<span data-ttu-id="c8730-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c8730-117">Application</span></span>|<span data-ttu-id="c8730-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c8730-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8730-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c8730-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="c8730-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c8730-120">Request headers</span></span>
|<span data-ttu-id="c8730-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c8730-121">Header</span></span>|<span data-ttu-id="c8730-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c8730-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8730-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c8730-123">Authorization</span></span>|<span data-ttu-id="c8730-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c8730-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8730-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c8730-125">Accept</span></span>|<span data-ttu-id="c8730-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8730-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8730-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c8730-127">Request body</span></span>
<span data-ttu-id="c8730-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c8730-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8730-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8730-129">Response</span></span>
<span data-ttu-id="c8730-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c8730-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8730-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c8730-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8730-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c8730-132">Request</span></span>
<span data-ttu-id="c8730-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c8730-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="c8730-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c8730-134">Response</span></span>
<span data-ttu-id="c8730-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c8730-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```




