---
title: Obter windowsInformationProtectionAppLockerFile
description: Ler propriedades e relações do objeto windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: feedd7eb216542ce14b263058c65b94729fa909d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022467"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="eee72-103">Obter windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="eee72-103">Get windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="eee72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eee72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eee72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eee72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eee72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eee72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eee72-107">Ler propriedades e relações do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="eee72-107">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eee72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eee72-108">Prerequisites</span></span>
<span data-ttu-id="eee72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eee72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eee72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eee72-111">Permission type</span></span>|<span data-ttu-id="eee72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eee72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eee72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eee72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eee72-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eee72-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eee72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eee72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eee72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eee72-116">Not supported.</span></span>|
|<span data-ttu-id="eee72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eee72-117">Application</span></span>|<span data-ttu-id="eee72-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eee72-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eee72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eee72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eee72-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eee72-120">Optional query parameters</span></span>
<span data-ttu-id="eee72-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eee72-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eee72-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eee72-122">Request headers</span></span>
|<span data-ttu-id="eee72-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eee72-123">Header</span></span>|<span data-ttu-id="eee72-124">Valor</span><span class="sxs-lookup"><span data-stu-id="eee72-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eee72-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eee72-125">Authorization</span></span>|<span data-ttu-id="eee72-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eee72-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eee72-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eee72-127">Accept</span></span>|<span data-ttu-id="eee72-128">application/json</span><span class="sxs-lookup"><span data-stu-id="eee72-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eee72-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eee72-129">Request body</span></span>
<span data-ttu-id="eee72-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eee72-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eee72-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee72-131">Response</span></span>
<span data-ttu-id="eee72-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eee72-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eee72-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eee72-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="eee72-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eee72-134">Request</span></span>
<span data-ttu-id="eee72-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eee72-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="eee72-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="eee72-136">Response</span></span>
<span data-ttu-id="eee72-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eee72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```






