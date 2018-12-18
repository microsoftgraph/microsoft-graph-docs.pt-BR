---
title: ação de importDeviceIdentityList
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: d3f719a9f2b7358acfa413810b6bd091d32f52f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338161"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="7874b-103">ação de importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="7874b-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="7874b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7874b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7874b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7874b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7874b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7874b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7874b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7874b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7874b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7874b-108">Prerequisites</span></span>
<span data-ttu-id="7874b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7874b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7874b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7874b-111">Permission type</span></span>|<span data-ttu-id="7874b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7874b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7874b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7874b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7874b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7874b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7874b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7874b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7874b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7874b-116">Not supported.</span></span>|
|<span data-ttu-id="7874b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7874b-117">Application</span></span>|<span data-ttu-id="7874b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7874b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7874b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7874b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="7874b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7874b-120">Request headers</span></span>
|<span data-ttu-id="7874b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7874b-121">Header</span></span>|<span data-ttu-id="7874b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7874b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7874b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7874b-123">Authorization</span></span>|<span data-ttu-id="7874b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7874b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7874b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7874b-125">Accept</span></span>|<span data-ttu-id="7874b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7874b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7874b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7874b-127">Request body</span></span>
<span data-ttu-id="7874b-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7874b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7874b-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7874b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7874b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7874b-130">Property</span></span>|<span data-ttu-id="7874b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7874b-131">Type</span></span>|<span data-ttu-id="7874b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7874b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7874b-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="7874b-133">importedDeviceIdentities</span></span>|<span data-ttu-id="7874b-134">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="7874b-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="7874b-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7874b-135">Not yet documented</span></span>|
|<span data-ttu-id="7874b-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="7874b-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="7874b-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="7874b-137">Boolean</span></span>|<span data-ttu-id="7874b-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7874b-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7874b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7874b-139">Response</span></span>
<span data-ttu-id="7874b-140">Se tiver êxito, essa ação retornará um `200 OK` código de resposta e um conjunto de [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7874b-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7874b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7874b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="7874b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7874b-142">Request</span></span>
<span data-ttu-id="7874b-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7874b-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7874b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7874b-144">Response</span></span>
<span data-ttu-id="7874b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7874b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





