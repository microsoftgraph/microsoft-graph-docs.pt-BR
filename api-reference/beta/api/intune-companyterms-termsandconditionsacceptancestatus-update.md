---
title: Atualizar termsAndConditionsAcceptanceStatus
description: Atualizar as propriedades de um objeto termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9149578ab470e29fa31877cb0e2a94994d3bc9d3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971903"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="dbca0-103">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="dbca0-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="dbca0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dbca0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbca0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbca0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbca0-106">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbca0-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbca0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dbca0-107">Prerequisites</span></span>
<span data-ttu-id="dbca0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbca0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbca0-110">Permission type</span></span>|<span data-ttu-id="dbca0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbca0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbca0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbca0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbca0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbca0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dbca0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbca0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbca0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbca0-115">Not supported.</span></span>|
|<span data-ttu-id="dbca0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbca0-116">Application</span></span>|<span data-ttu-id="dbca0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbca0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbca0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbca0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="dbca0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbca0-119">Request headers</span></span>
|<span data-ttu-id="dbca0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dbca0-120">Header</span></span>|<span data-ttu-id="dbca0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dbca0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbca0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbca0-122">Authorization</span></span>|<span data-ttu-id="dbca0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbca0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbca0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dbca0-124">Accept</span></span>|<span data-ttu-id="dbca0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dbca0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbca0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbca0-126">Request body</span></span>
<span data-ttu-id="dbca0-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbca0-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="dbca0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dbca0-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="dbca0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbca0-129">Property</span></span>|<span data-ttu-id="dbca0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbca0-130">Type</span></span>|<span data-ttu-id="dbca0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbca0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbca0-132">id</span><span class="sxs-lookup"><span data-stu-id="dbca0-132">id</span></span>|<span data-ttu-id="dbca0-133">String</span><span class="sxs-lookup"><span data-stu-id="dbca0-133">String</span></span>|<span data-ttu-id="dbca0-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="dbca0-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="dbca0-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dbca0-135">userDisplayName</span></span>|<span data-ttu-id="dbca0-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbca0-136">String</span></span>|<span data-ttu-id="dbca0-137">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="dbca0-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="dbca0-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="dbca0-138">acceptedVersion</span></span>|<span data-ttu-id="dbca0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="dbca0-139">Int32</span></span>|<span data-ttu-id="dbca0-140">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="dbca0-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="dbca0-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbca0-141">acceptedDateTime</span></span>|<span data-ttu-id="dbca0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbca0-142">DateTimeOffset</span></span>|<span data-ttu-id="dbca0-143">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="dbca0-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="dbca0-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbca0-144">Response</span></span>
<span data-ttu-id="dbca0-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbca0-145">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbca0-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbca0-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbca0-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbca0-147">Request</span></span>
<span data-ttu-id="dbca0-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dbca0-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="dbca0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbca0-149">Response</span></span>
<span data-ttu-id="dbca0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbca0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





