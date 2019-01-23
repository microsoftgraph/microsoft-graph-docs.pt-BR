---
title: Obter windowsInformationProtectionAppLockerFile
description: Ler propriedades e relações do objeto windowsInformationProtectionAppLockerFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf563c5e4afbec829803c3fc78029990e0a08f50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414988"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="5d302-103">Obter windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="5d302-103">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="5d302-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5d302-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d302-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5d302-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d302-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5d302-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d302-107">Ler propriedades e relações do objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5d302-107">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d302-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5d302-108">Prerequisites</span></span>
<span data-ttu-id="5d302-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d302-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5d302-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d302-111">Permission type</span></span>|<span data-ttu-id="5d302-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5d302-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d302-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d302-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d302-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d302-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5d302-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d302-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d302-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d302-116">Not supported.</span></span>|
|<span data-ttu-id="5d302-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d302-117">Application</span></span>|<span data-ttu-id="5d302-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d302-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d302-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d302-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="5d302-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d302-120">Optional query parameters</span></span>
<span data-ttu-id="5d302-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d302-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d302-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d302-122">Request headers</span></span>
|<span data-ttu-id="5d302-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5d302-123">Header</span></span>|<span data-ttu-id="5d302-124">Valor</span><span class="sxs-lookup"><span data-stu-id="5d302-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d302-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d302-125">Authorization</span></span>|<span data-ttu-id="5d302-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d302-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d302-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5d302-127">Accept</span></span>|<span data-ttu-id="5d302-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5d302-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d302-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d302-129">Request body</span></span>
<span data-ttu-id="5d302-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d302-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d302-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d302-131">Response</span></span>
<span data-ttu-id="5d302-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d302-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d302-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d302-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d302-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d302-134">Request</span></span>
<span data-ttu-id="5d302-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d302-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="5d302-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d302-136">Response</span></span>
<span data-ttu-id="5d302-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d302-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




