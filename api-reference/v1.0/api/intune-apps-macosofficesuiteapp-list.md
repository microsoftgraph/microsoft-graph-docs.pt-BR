---
title: Listar macOSOfficeSuiteApps
description: Listar propriedades e relações dos objetos macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05afa8f0794cb263dd9c36b7d21cbd1178559c26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577228"
---
# <a name="list-macosofficesuiteapps"></a><span data-ttu-id="ed5f0-103">Listar macOSOfficeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="ed5f0-103">List macOSOfficeSuiteApps</span></span>

> <span data-ttu-id="ed5f0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed5f0-105">Listar propriedades e relações dos objetos [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ed5f0-105">List properties and relationships of the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed5f0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed5f0-106">Prerequisites</span></span>
<span data-ttu-id="ed5f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed5f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed5f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed5f0-109">Permission type</span></span>|<span data-ttu-id="ed5f0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed5f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed5f0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed5f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed5f0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed5f0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ed5f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed5f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed5f0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-114">Not supported.</span></span>|
|<span data-ttu-id="ed5f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed5f0-115">Application</span></span>|<span data-ttu-id="ed5f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed5f0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed5f0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ed5f0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5f0-118">Request headers</span></span>
|<span data-ttu-id="ed5f0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed5f0-119">Header</span></span>|<span data-ttu-id="ed5f0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ed5f0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed5f0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed5f0-121">Authorization</span></span>|<span data-ttu-id="ed5f0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed5f0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed5f0-123">Accept</span></span>|<span data-ttu-id="ed5f0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ed5f0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed5f0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5f0-125">Request body</span></span>
<span data-ttu-id="ed5f0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed5f0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed5f0-127">Response</span></span>
<span data-ttu-id="ed5f0-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-128">If successful, this method returns a `200 OK` response code and a collection of [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed5f0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed5f0-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed5f0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed5f0-130">Request</span></span>
<span data-ttu-id="ed5f0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="ed5f0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed5f0-132">Response</span></span>
<span data-ttu-id="ed5f0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed5f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 865

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
      "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "processing"
    }
  ]
}
```



