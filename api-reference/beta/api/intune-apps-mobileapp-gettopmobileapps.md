---
title: função getTopMobileApps
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f5a380145c51ba61fe76638941c42352f254606e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980206"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="9fc05-103">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="9fc05-103">getTopMobileApps function</span></span>

> <span data-ttu-id="9fc05-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9fc05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fc05-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9fc05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fc05-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9fc05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fc05-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fc05-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fc05-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fc05-108">Prerequisites</span></span>
<span data-ttu-id="9fc05-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc05-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fc05-111">Permission type</span></span>|<span data-ttu-id="9fc05-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fc05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fc05-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fc05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fc05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9fc05-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9fc05-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fc05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fc05-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fc05-116">Not supported.</span></span>|
|<span data-ttu-id="9fc05-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fc05-117">Application</span></span>|<span data-ttu-id="9fc05-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fc05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fc05-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9fc05-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc05-120">Request headers</span></span>
|<span data-ttu-id="9fc05-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fc05-121">Header</span></span>|<span data-ttu-id="9fc05-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9fc05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fc05-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fc05-123">Authorization</span></span>|<span data-ttu-id="9fc05-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fc05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fc05-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9fc05-125">Accept</span></span>|<span data-ttu-id="9fc05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fc05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fc05-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc05-127">Request body</span></span>
<span data-ttu-id="9fc05-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9fc05-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9fc05-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9fc05-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9fc05-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fc05-130">Property</span></span>|<span data-ttu-id="9fc05-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fc05-131">Type</span></span>|<span data-ttu-id="9fc05-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fc05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fc05-133">status</span><span class="sxs-lookup"><span data-stu-id="9fc05-133">status</span></span>|<span data-ttu-id="9fc05-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fc05-134">String</span></span>|<span data-ttu-id="9fc05-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fc05-135">Not yet documented</span></span>|
|<span data-ttu-id="9fc05-136">count</span><span class="sxs-lookup"><span data-stu-id="9fc05-136">count</span></span>|<span data-ttu-id="9fc05-137">Int64</span><span class="sxs-lookup"><span data-stu-id="9fc05-137">Int64</span></span>|<span data-ttu-id="9fc05-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9fc05-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9fc05-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fc05-139">Response</span></span>
<span data-ttu-id="9fc05-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um conjunto de [mobileApp](../resources/intune-apps-mobileapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fc05-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fc05-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fc05-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fc05-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fc05-142">Request</span></span>
<span data-ttu-id="9fc05-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fc05-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="9fc05-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fc05-144">Response</span></span>
<span data-ttu-id="9fc05-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fc05-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 881

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      "uploadState": 11,
      "publishingState": "processing"
    }
  ]
}
```





