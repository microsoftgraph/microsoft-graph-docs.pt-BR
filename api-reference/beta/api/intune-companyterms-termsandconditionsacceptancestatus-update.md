---
title: Atualizar termsAndConditionsAcceptanceStatus
description: Atualizar as propriedades de um objeto termsAndConditionsAcceptanceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a888767b3ee8d027d6ef7cde22778505dd818360
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760113"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="624df-103">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="624df-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="624df-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="624df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="624df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="624df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="624df-106">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="624df-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="624df-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="624df-107">Prerequisites</span></span>
<span data-ttu-id="624df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="624df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="624df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="624df-110">Permission type</span></span>|<span data-ttu-id="624df-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="624df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="624df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="624df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="624df-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="624df-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="624df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="624df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="624df-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="624df-115">Not supported.</span></span>|
|<span data-ttu-id="624df-116">Application</span><span class="sxs-lookup"><span data-stu-id="624df-116">Application</span></span>|<span data-ttu-id="624df-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="624df-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="624df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="624df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="624df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="624df-119">Request headers</span></span>
|<span data-ttu-id="624df-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="624df-120">Header</span></span>|<span data-ttu-id="624df-121">Valor</span><span class="sxs-lookup"><span data-stu-id="624df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="624df-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="624df-122">Authorization</span></span>|<span data-ttu-id="624df-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="624df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="624df-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="624df-124">Accept</span></span>|<span data-ttu-id="624df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="624df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="624df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="624df-126">Request body</span></span>
<span data-ttu-id="624df-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="624df-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="624df-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="624df-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="624df-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="624df-129">Property</span></span>|<span data-ttu-id="624df-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="624df-130">Type</span></span>|<span data-ttu-id="624df-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="624df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="624df-132">id</span><span class="sxs-lookup"><span data-stu-id="624df-132">id</span></span>|<span data-ttu-id="624df-133">String</span><span class="sxs-lookup"><span data-stu-id="624df-133">String</span></span>|<span data-ttu-id="624df-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="624df-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="624df-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="624df-135">userDisplayName</span></span>|<span data-ttu-id="624df-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="624df-136">String</span></span>|<span data-ttu-id="624df-137">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="624df-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="624df-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="624df-138">acceptedVersion</span></span>|<span data-ttu-id="624df-139">Int32</span><span class="sxs-lookup"><span data-stu-id="624df-139">Int32</span></span>|<span data-ttu-id="624df-140">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="624df-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="624df-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="624df-141">acceptedDateTime</span></span>|<span data-ttu-id="624df-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="624df-142">DateTimeOffset</span></span>|<span data-ttu-id="624df-143">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="624df-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="624df-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="624df-144">userPrincipalName</span></span>|<span data-ttu-id="624df-145">String</span><span class="sxs-lookup"><span data-stu-id="624df-145">String</span></span>|<span data-ttu-id="624df-146">O userPrincipalName do usuário que aceitou o termo.</span><span class="sxs-lookup"><span data-stu-id="624df-146">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="624df-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="624df-147">Response</span></span>
<span data-ttu-id="624df-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="624df-148">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="624df-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="624df-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="624df-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="624df-150">Request</span></span>
<span data-ttu-id="624df-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="624df-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="624df-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="624df-152">Response</span></span>
<span data-ttu-id="624df-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="624df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




