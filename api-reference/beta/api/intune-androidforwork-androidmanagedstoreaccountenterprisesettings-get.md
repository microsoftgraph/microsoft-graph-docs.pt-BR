---
title: Obter androidManagedStoreAccountEnterpriseSettings
description: Leia as propriedades e as relações do objeto androidManagedStoreAccountEnterpriseSettings.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 173fdb387d1dfe99dae8eaf7e464511dca1e0bda
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762500"
---
# <a name="get-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="1c8a6-103">Obter androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="1c8a6-103">Get androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="1c8a6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c8a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c8a6-106">Leia as propriedades e as relações do objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="1c8a6-106">Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c8a6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c8a6-107">Prerequisites</span></span>
<span data-ttu-id="1c8a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c8a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c8a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c8a6-110">Permission type</span></span>|<span data-ttu-id="1c8a6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c8a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c8a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c8a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c8a6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c8a6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c8a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c8a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c8a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-115">Not supported.</span></span>|
|<span data-ttu-id="1c8a6-116">Application</span><span class="sxs-lookup"><span data-stu-id="1c8a6-116">Application</span></span>|<span data-ttu-id="1c8a6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c8a6-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c8a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c8a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c8a6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c8a6-119">Optional query parameters</span></span>
<span data-ttu-id="1c8a6-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c8a6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c8a6-121">Request headers</span></span>
|<span data-ttu-id="1c8a6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c8a6-122">Header</span></span>|<span data-ttu-id="1c8a6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1c8a6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c8a6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c8a6-124">Authorization</span></span>|<span data-ttu-id="1c8a6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c8a6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c8a6-126">Accept</span></span>|<span data-ttu-id="1c8a6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1c8a6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c8a6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c8a6-128">Request body</span></span>
<span data-ttu-id="1c8a6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c8a6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c8a6-130">Response</span></span>
<span data-ttu-id="1c8a6-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c8a6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c8a6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c8a6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c8a6-133">Request</span></span>
<span data-ttu-id="1c8a6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

### <a name="response"></a><span data-ttu-id="1c8a6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c8a6-135">Response</span></span>
<span data-ttu-id="1c8a6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c8a6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1081

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
    "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true,
    "companyCodes": [
      {
        "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
        "enrollmentToken": "Enrollment Token value",
        "qrCodeContent": "Qr Code Content value",
        "qrCodeImage": {
          "@odata.type": "microsoft.graph.mimeContent",
          "type": "Type value",
          "value": "dmFsdWU="
        }
      }
    ],
    "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
  }
}
```




