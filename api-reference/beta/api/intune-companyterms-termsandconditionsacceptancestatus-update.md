---
title: Atualizar termsAndConditionsAcceptanceStatus
description: Atualizar as propriedades de um objeto termsAndConditionsAcceptanceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a09b95a815a37994ce10827ac304e9ab377d51fe
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159140"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="4ffc5-103">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="4ffc5-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="4ffc5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ffc5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ffc5-106">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4ffc5-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ffc5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ffc5-107">Prerequisites</span></span>
<span data-ttu-id="4ffc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ffc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ffc5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ffc5-110">Permission type</span></span>|<span data-ttu-id="4ffc5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ffc5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ffc5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ffc5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ffc5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ffc5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4ffc5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ffc5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ffc5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-115">Not supported.</span></span>|
|<span data-ttu-id="4ffc5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ffc5-116">Application</span></span>|<span data-ttu-id="4ffc5-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ffc5-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ffc5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ffc5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4ffc5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ffc5-119">Request headers</span></span>
|<span data-ttu-id="4ffc5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ffc5-120">Header</span></span>|<span data-ttu-id="4ffc5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4ffc5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ffc5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ffc5-122">Authorization</span></span>|<span data-ttu-id="4ffc5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ffc5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ffc5-124">Accept</span></span>|<span data-ttu-id="4ffc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ffc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ffc5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ffc5-126">Request body</span></span>
<span data-ttu-id="4ffc5-127">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4ffc5-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="4ffc5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4ffc5-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="4ffc5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ffc5-129">Property</span></span>|<span data-ttu-id="4ffc5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ffc5-130">Type</span></span>|<span data-ttu-id="4ffc5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ffc5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ffc5-132">id</span><span class="sxs-lookup"><span data-stu-id="4ffc5-132">id</span></span>|<span data-ttu-id="4ffc5-133">String</span><span class="sxs-lookup"><span data-stu-id="4ffc5-133">String</span></span>|<span data-ttu-id="4ffc5-134">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="4ffc5-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4ffc5-135">userDisplayName</span></span>|<span data-ttu-id="4ffc5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ffc5-136">String</span></span>|<span data-ttu-id="4ffc5-137">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="4ffc5-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="4ffc5-138">acceptedVersion</span></span>|<span data-ttu-id="4ffc5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4ffc5-139">Int32</span></span>|<span data-ttu-id="4ffc5-140">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="4ffc5-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ffc5-141">acceptedDateTime</span></span>|<span data-ttu-id="4ffc5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ffc5-142">DateTimeOffset</span></span>|<span data-ttu-id="4ffc5-143">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-143">DateTime when the terms were last accepted by the user.</span></span>|
|<span data-ttu-id="4ffc5-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4ffc5-144">userPrincipalName</span></span>|<span data-ttu-id="4ffc5-145">String</span><span class="sxs-lookup"><span data-stu-id="4ffc5-145">String</span></span>|<span data-ttu-id="4ffc5-146">O userPrincipalName do usuário que aceitou o termo.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-146">The userPrincipalName of the User that accepted the term.</span></span>|



## <a name="response"></a><span data-ttu-id="4ffc5-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ffc5-147">Response</span></span>
<span data-ttu-id="4ffc5-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-148">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ffc5-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ffc5-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ffc5-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ffc5-150">Request</span></span>
<span data-ttu-id="4ffc5-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ffc5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ffc5-152">Response</span></span>
<span data-ttu-id="4ffc5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ffc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





