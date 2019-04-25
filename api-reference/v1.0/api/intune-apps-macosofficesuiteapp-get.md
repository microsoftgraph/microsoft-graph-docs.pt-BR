---
title: Acessar macOSOfficeSuiteApp
description: Leia as propriedades e as relações do objeto macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6511aada777e7fcd6e4df7728b604cea49702e05
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577186"
---
# <a name="get-macosofficesuiteapp"></a><span data-ttu-id="fa7cb-103">Acessar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="fa7cb-103">Get macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="fa7cb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa7cb-105">Leia as propriedades e as relações do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="fa7cb-105">Read properties and relationships of the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa7cb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa7cb-106">Prerequisites</span></span>
<span data-ttu-id="fa7cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa7cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa7cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa7cb-109">Permission type</span></span>|<span data-ttu-id="fa7cb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa7cb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa7cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa7cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa7cb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa7cb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa7cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa7cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa7cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-114">Not supported.</span></span>|
|<span data-ttu-id="fa7cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa7cb-115">Application</span></span>|<span data-ttu-id="fa7cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa7cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa7cb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa7cb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa7cb-118">Optional query parameters</span></span>
<span data-ttu-id="fa7cb-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa7cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa7cb-120">Request headers</span></span>
|<span data-ttu-id="fa7cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa7cb-121">Header</span></span>|<span data-ttu-id="fa7cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fa7cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa7cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa7cb-123">Authorization</span></span>|<span data-ttu-id="fa7cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa7cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa7cb-125">Accept</span></span>|<span data-ttu-id="fa7cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa7cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa7cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa7cb-127">Request body</span></span>
<span data-ttu-id="fa7cb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa7cb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa7cb-129">Response</span></span>
<span data-ttu-id="fa7cb-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-130">If successful, this method returns a `200 OK` response code and [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa7cb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa7cb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa7cb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa7cb-132">Request</span></span>
<span data-ttu-id="fa7cb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="fa7cb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa7cb-134">Response</span></span>
<span data-ttu-id="fa7cb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa7cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 813

{
  "value": {
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
}
```



