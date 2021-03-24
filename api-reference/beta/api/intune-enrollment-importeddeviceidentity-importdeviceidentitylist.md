---
title: Ação importDeviceIdentityList
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cabdebeba97764754864fb087127f3d47bfd5c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142335"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="d673c-103">Ação importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="d673c-103">importDeviceIdentityList action</span></span>

<span data-ttu-id="d673c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d673c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d673c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d673c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d673c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d673c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d673c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d673c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d673c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d673c-108">Prerequisites</span></span>
<span data-ttu-id="d673c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d673c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d673c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d673c-111">Permission type</span></span>|<span data-ttu-id="d673c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d673c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d673c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d673c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d673c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d673c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d673c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d673c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d673c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d673c-116">Not supported.</span></span>|
|<span data-ttu-id="d673c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d673c-117">Application</span></span>|<span data-ttu-id="d673c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d673c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d673c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d673c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="d673c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d673c-120">Request headers</span></span>
|<span data-ttu-id="d673c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d673c-121">Header</span></span>|<span data-ttu-id="d673c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d673c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d673c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d673c-123">Authorization</span></span>|<span data-ttu-id="d673c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d673c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d673c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d673c-125">Accept</span></span>|<span data-ttu-id="d673c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d673c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d673c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d673c-127">Request body</span></span>
<span data-ttu-id="d673c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d673c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d673c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d673c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d673c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d673c-130">Property</span></span>|<span data-ttu-id="d673c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d673c-131">Type</span></span>|<span data-ttu-id="d673c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d673c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d673c-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="d673c-133">importedDeviceIdentities</span></span>|<span data-ttu-id="d673c-134">[Coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d673c-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="d673c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d673c-135">Not yet documented</span></span>|
|<span data-ttu-id="d673c-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="d673c-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="d673c-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="d673c-137">Boolean</span></span>|<span data-ttu-id="d673c-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d673c-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d673c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d673c-139">Response</span></span>
<span data-ttu-id="d673c-140">Se tiver êxito, essa ação retornará um código de resposta e uma `200 OK` [coleção importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d673c-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d673c-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d673c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d673c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d673c-142">Request</span></span>
<span data-ttu-id="d673c-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d673c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="d673c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d673c-144">Response</span></span>
<span data-ttu-id="d673c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d673c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```




