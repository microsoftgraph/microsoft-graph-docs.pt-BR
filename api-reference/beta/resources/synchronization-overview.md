---
title: Visão geral da API de sincronização do Azure AD
description: Automatize o provisionamento de identidades de sistemas de RH, Active Directory e Azure Active Directory para aplicativos em nuvem.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a08be511c3752e27f2e86415aee62d112d2c5262
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133158"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="c7901-103">Visão geral da API de sincronização do Azure AD</span><span class="sxs-lookup"><span data-stu-id="c7901-103">Azure AD synchronization API overview</span></span>

<span data-ttu-id="c7901-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7901-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7901-105">A sincronização de identidade do Azure Active Directory (Azure AD) (também chamada de "provisionamento") permite automatizar o provisionamento (criação, manutenção) e o des provisionamento (remoção) de identidades de qualquer um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="c7901-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the provisioning (creation, maintenance) and de-provisioning (removal) of identities from any of the following:</span></span>
- <span data-ttu-id="c7901-106">Active Directory para Azure AD</span><span class="sxs-lookup"><span data-stu-id="c7901-106">Active Directory to Azure AD</span></span>
- <span data-ttu-id="c7901-107">Dia de trabalho para o Azure AD</span><span class="sxs-lookup"><span data-stu-id="c7901-107">Workday to Azure AD</span></span>
- <span data-ttu-id="c7901-108">Azure AD para aplicativos de nuvem como Dropbox, Salesforce, ServiceNow e muito mais</span><span class="sxs-lookup"><span data-stu-id="c7901-108">Azure AD to cloud applications such as Dropbox, Salesforce, ServiceNow, and more</span></span> 

<span data-ttu-id="c7901-109">Você pode usar as APIs de sincronização  no Microsoft Graph para gerenciar a sincronização de identidade programaticamente, incluindo:</span><span class="sxs-lookup"><span data-stu-id="c7901-109">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="c7901-110">Criar, iniciar e interromper trabalhos de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-110">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="c7901-111">Fazer alterações no esquema de sincronização para trabalhos</span><span class="sxs-lookup"><span data-stu-id="c7901-111">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="c7901-112">Status de sincronização atual.</span><span class="sxs-lookup"><span data-stu-id="c7901-112">Verify the current synchronization status</span></span>

<span data-ttu-id="c7901-113">Para saber mais sobre a sincronização no Azure AD, confira:</span><span class="sxs-lookup"><span data-stu-id="c7901-113">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="c7901-114">Automatizar o provisionamento e o desprovisionamento de usuários para aplicativos SaaS com o Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c7901-114">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="c7901-115">Gerenciando o provisionamento de conta de usuário para aplicativos corporativos no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="c7901-115">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="c7901-116">Você também pode experimentar a API no Explorador do [Graph em](https://developer.microsoft.com/graph/graph-explorer) um locatário de exemplo ou em seu próprio locatário.</span><span class="sxs-lookup"><span data-stu-id="c7901-116">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="c7901-117">Trabalho de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-117">Synchronization job</span></span>

<span data-ttu-id="c7901-118">Os trabalhos de sincronização executam a sincronização periodicamente em segundo plano, sondando alterações em um diretório e os pressionando para outro diretório.</span><span class="sxs-lookup"><span data-stu-id="c7901-118">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="c7901-119">O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="c7901-119">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="c7901-120">Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="c7901-120">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="c7901-121">Para obter mais informações, consulte [o trabalho de sincronização.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="c7901-121">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="c7901-122">Esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-122">Synchronization schema</span></span>

<span data-ttu-id="c7901-123">O esquema de sincronização define quais objetos serão sincronizados e como eles serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="c7901-123">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="c7901-124">O esquema de sincronização contém a maioria das informações de configuração para um trabalho de sincronização específico.</span><span class="sxs-lookup"><span data-stu-id="c7901-124">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="c7901-125">Normalmente, você personalizará alguns dos [mapeamentos](synchronization-attributemapping.md)de atributos ou adicionará um filtro de [scoping](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.</span><span class="sxs-lookup"><span data-stu-id="c7901-125">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="c7901-126">O esquema de sincronização inclui os seguintes componentes:</span><span class="sxs-lookup"><span data-stu-id="c7901-126">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="c7901-127">Definições de diretório</span><span class="sxs-lookup"><span data-stu-id="c7901-127">Directory definitions</span></span>
- <span data-ttu-id="c7901-128">Regras de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-128">Synchronization rules</span></span>
- <span data-ttu-id="c7901-129">Mapeamentos de objetos</span><span class="sxs-lookup"><span data-stu-id="c7901-129">Object mappings</span></span>

<span data-ttu-id="c7901-130">Para obter mais informações, [consulte o esquema de sincronização.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="c7901-130">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="c7901-131">Modelo de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-131">Synchronization template</span></span>

<span data-ttu-id="c7901-132">O modelo de sincronização fornece configurações de sincronização pré-configuradas para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="c7901-132">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="c7901-133">Essas configurações (o mais [importante,](synchronization-synchronizationschema.md)esquema de sincronização [](synchronization-synchronizationjob.md) ) serão usadas por padrão para qualquer trabalho de sincronização baseado no modelo.</span><span class="sxs-lookup"><span data-stu-id="c7901-133">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="c7901-134">Os modelos são especificados pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7901-134">Templates are specified by the application developer.</span></span>

<span data-ttu-id="c7901-135">Para obter mais informações, consulte [o modelo de sincronização.](synchronization-synchronizationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c7901-135">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="c7901-136">Trabalhando com a API de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-136">Working with the synchronization API</span></span>

<span data-ttu-id="c7901-137">Trabalhar com a API de sincronização envolve principalmente o acesso aos recursos [synchronizationJob](synchronization-synchronizationjob.md) e [synchronizationSchema.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="c7901-137">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="c7901-138">Para encontrar o [recurso synchronizationJob,](synchronization-synchronizationjob.md) você precisa saber a ID do objeto de entidade de serviço ao qual o trabalho de sincronização pertence.</span><span class="sxs-lookup"><span data-stu-id="c7901-138">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="c7901-139">Os exemplos a seguir mostram como trabalhar com os recursos **synchronizationJob** e **synchronizationSchema.**</span><span class="sxs-lookup"><span data-stu-id="c7901-139">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="c7901-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7901-140">Authorization</span></span>

<span data-ttu-id="c7901-141">A API de sincronização do Azure AD usa o OAuth 2.0 para autorização.</span><span class="sxs-lookup"><span data-stu-id="c7901-141">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="c7901-142">Antes de fazer solicitações à API, você precisa obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="c7901-142">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="c7901-143">Para saber mais, confira [Obter tokens de acesso para chamar o Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="c7901-143">For more information, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span> <span data-ttu-id="c7901-144">Para acessar os recursos de sincronização, seu aplicativo precisa de permissões Directory.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c7901-144">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="c7901-145">Para obter mais informações, consulte [Permissões de diretório.](/graph/permissions-reference#directory-permissions)</span><span class="sxs-lookup"><span data-stu-id="c7901-145">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="c7901-146">Encontrar o objeto de entidade de serviço por nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c7901-146">Find the service principal object by display name</span></span>

<span data-ttu-id="c7901-147">O exemplo a seguir mostra como encontrar o objeto de entidade de serviço pelo nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="c7901-147">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="c7901-148">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c7901-148">**Request**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="c7901-149">**Response**</span><span class="sxs-lookup"><span data-stu-id="c7901-149">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="c7901-150">Encontre o objeto da entidade de serviço por ID do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7901-150">Find the service principal object by app ID</span></span>

<span data-ttu-id="c7901-151">O exemplo a seguir mostra como encontrar o objeto de entidade de serviço por ID do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c7901-151">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="c7901-152">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c7901-152">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="c7901-153">**Response**</span><span class="sxs-lookup"><span data-stu-id="c7901-153">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="c7901-154">Listar trabalhos de sincronização existentes</span><span class="sxs-lookup"><span data-stu-id="c7901-154">List existing synchronization jobs</span></span>

<span data-ttu-id="c7901-155">O exemplo a seguir mostra como listar trabalhos de sincronização existentes.</span><span class="sxs-lookup"><span data-stu-id="c7901-155">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="c7901-156">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c7901-156">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="c7901-157">**Response**</span><span class="sxs-lookup"><span data-stu-id="c7901-157">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="c7901-158">Obter status do trabalho de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-158">Get synchronization job status</span></span>
<span data-ttu-id="c7901-159">O exemplo a seguir mostra como obter o status de um trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c7901-159">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="c7901-160">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c7901-160">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="c7901-161">**Response**</span><span class="sxs-lookup"><span data-stu-id="c7901-161">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="c7901-162">Obter esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="c7901-162">Get synchronization schema</span></span>
<span data-ttu-id="c7901-163">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="c7901-163">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="c7901-164">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c7901-164">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="c7901-165">**Response**</span><span class="sxs-lookup"><span data-stu-id="c7901-165">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="c7901-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="c7901-166">See also</span></span>

* [<span data-ttu-id="c7901-167">Configurar a sincronização com atributos de extensão de diretório</span><span class="sxs-lookup"><span data-stu-id="c7901-167">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="c7901-168">Configurar a sincronização com atributos de destino personalizados</span><span class="sxs-lookup"><span data-stu-id="c7901-168">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)
