---
title: Criar officeSuiteApp
description: Crie um novo objeto de officeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1821c88f974bf61fe23de6bb34cfeb06d9250f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405839"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="4a3e9-103">Criar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="4a3e9-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="4a3e9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a3e9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a3e9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a3e9-107">Crie um novo objeto de [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4a3e9-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a3e9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a3e9-108">Prerequisites</span></span>
<span data-ttu-id="4a3e9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a3e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a3e9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a3e9-111">Permission type</span></span>|<span data-ttu-id="4a3e9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a3e9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a3e9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a3e9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a3e9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a3e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-116">Not supported.</span></span>|
|<span data-ttu-id="4a3e9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a3e9-117">Application</span></span>|<span data-ttu-id="4a3e9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a3e9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a3e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4a3e9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a3e9-120">Request headers</span></span>
|<span data-ttu-id="4a3e9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a3e9-121">Header</span></span>|<span data-ttu-id="4a3e9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a3e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a3e9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a3e9-123">Authorization</span></span>|<span data-ttu-id="4a3e9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a3e9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a3e9-125">Accept</span></span>|<span data-ttu-id="4a3e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a3e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a3e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a3e9-127">Request body</span></span>
<span data-ttu-id="4a3e9-128">No corpo da solicitação, fornece uma representação JSON para o objeto officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="4a3e9-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="4a3e9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a3e9-130">Property</span></span>|<span data-ttu-id="4a3e9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a3e9-131">Type</span></span>|<span data-ttu-id="4a3e9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a3e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a3e9-133">id</span><span class="sxs-lookup"><span data-stu-id="4a3e9-133">id</span></span>|<span data-ttu-id="4a3e9-134">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-134">String</span></span>|<span data-ttu-id="4a3e9-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-135">Key of the entity.</span></span> <span data-ttu-id="4a3e9-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4a3e9-137">displayName</span></span>|<span data-ttu-id="4a3e9-138">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-138">String</span></span>|<span data-ttu-id="4a3e9-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4a3e9-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-141">description</span><span class="sxs-lookup"><span data-stu-id="4a3e9-141">description</span></span>|<span data-ttu-id="4a3e9-142">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-142">String</span></span>|<span data-ttu-id="4a3e9-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-143">The description of the app.</span></span> <span data-ttu-id="4a3e9-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4a3e9-145">publisher</span></span>|<span data-ttu-id="4a3e9-146">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-146">String</span></span>|<span data-ttu-id="4a3e9-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-147">The publisher of the app.</span></span> <span data-ttu-id="4a3e9-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4a3e9-149">largeIcon</span></span>|[<span data-ttu-id="4a3e9-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4a3e9-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4a3e9-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4a3e9-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a3e9-153">createdDateTime</span></span>|<span data-ttu-id="4a3e9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a3e9-154">DateTimeOffset</span></span>|<span data-ttu-id="4a3e9-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-155">The date and time the app was created.</span></span> <span data-ttu-id="4a3e9-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a3e9-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4a3e9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a3e9-158">DateTimeOffset</span></span>|<span data-ttu-id="4a3e9-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4a3e9-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4a3e9-161">isFeatured</span></span>|<span data-ttu-id="4a3e9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a3e9-162">Boolean</span></span>|<span data-ttu-id="4a3e9-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4a3e9-164">privacyInformationUrl</span></span>|<span data-ttu-id="4a3e9-165">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-165">String</span></span>|<span data-ttu-id="4a3e9-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-166">The privacy statement Url.</span></span> <span data-ttu-id="4a3e9-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4a3e9-168">informationUrl</span></span>|<span data-ttu-id="4a3e9-169">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-169">String</span></span>|<span data-ttu-id="4a3e9-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-170">The more information Url.</span></span> <span data-ttu-id="4a3e9-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-172">owner</span><span class="sxs-lookup"><span data-stu-id="4a3e9-172">owner</span></span>|<span data-ttu-id="4a3e9-173">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-173">String</span></span>|<span data-ttu-id="4a3e9-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-174">The owner of the app.</span></span> <span data-ttu-id="4a3e9-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-176">developer</span><span class="sxs-lookup"><span data-stu-id="4a3e9-176">developer</span></span>|<span data-ttu-id="4a3e9-177">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-177">String</span></span>|<span data-ttu-id="4a3e9-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-178">The developer of the app.</span></span> <span data-ttu-id="4a3e9-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-180">Observações</span><span class="sxs-lookup"><span data-stu-id="4a3e9-180">notes</span></span>|<span data-ttu-id="4a3e9-181">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-181">String</span></span>|<span data-ttu-id="4a3e9-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-182">Notes for the app.</span></span> <span data-ttu-id="4a3e9-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4a3e9-184">uploadState</span></span>|<span data-ttu-id="4a3e9-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4a3e9-185">Int32</span></span>|<span data-ttu-id="4a3e9-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-186">The upload state.</span></span> <span data-ttu-id="4a3e9-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4a3e9-188">publishingState</span></span>|[<span data-ttu-id="4a3e9-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4a3e9-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4a3e9-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-190">The publishing state for the app.</span></span> <span data-ttu-id="4a3e9-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4a3e9-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4a3e9-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4a3e9-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4a3e9-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4a3e9-194">isAssigned</span></span>|<span data-ttu-id="4a3e9-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a3e9-195">Boolean</span></span>|<span data-ttu-id="4a3e9-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4a3e9-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a3e9-198">roleScopeTagIds</span></span>|<span data-ttu-id="4a3e9-199">String collection</span><span class="sxs-lookup"><span data-stu-id="4a3e9-199">String collection</span></span>|<span data-ttu-id="4a3e9-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4a3e9-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4a3e9-202">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="4a3e9-202">autoAcceptEula</span></span>|<span data-ttu-id="4a3e9-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a3e9-203">Boolean</span></span>|<span data-ttu-id="4a3e9-204">O valor para aceitar o EULA automaticamente no dispositivo do usuário final.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-204">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="4a3e9-205">productIds</span><span class="sxs-lookup"><span data-stu-id="4a3e9-205">productIds</span></span>|<span data-ttu-id="4a3e9-206">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="4a3e9-206">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="4a3e9-207">As Ids de produto que representam a SKU do pacote Office365.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-207">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="4a3e9-208">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-208">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="4a3e9-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="4a3e9-209">excludedApps</span></span>|[<span data-ttu-id="4a3e9-210">excludedApps</span><span class="sxs-lookup"><span data-stu-id="4a3e9-210">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="4a3e9-211">A propriedade para representar os aplicativos que são excluídos do produto selecionado Office365 ID.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-211">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="4a3e9-212">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="4a3e9-212">useSharedComputerActivation</span></span>|<span data-ttu-id="4a3e9-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a3e9-213">Boolean</span></span>|<span data-ttu-id="4a3e9-214">A propriedade para representar que se a ativação do computador compartilhado é usada não para o pacote do app Office365.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-214">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="4a3e9-215">updateChannel</span><span class="sxs-lookup"><span data-stu-id="4a3e9-215">updateChannel</span></span>|[<span data-ttu-id="4a3e9-216">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="4a3e9-216">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="4a3e9-217">A propriedade para representar o canal de atualização Office365.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-217">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="4a3e9-218">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-218">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="4a3e9-219">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="4a3e9-219">officePlatformArchitecture</span></span>|[<span data-ttu-id="4a3e9-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4a3e9-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4a3e9-221">A propriedade para representar a versão do pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-221">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="4a3e9-222">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4a3e9-223">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="4a3e9-223">localesToInstall</span></span>|<span data-ttu-id="4a3e9-224">String collection</span><span class="sxs-lookup"><span data-stu-id="4a3e9-224">String collection</span></span>|<span data-ttu-id="4a3e9-225">A propriedade para representar as localidades que são instaladas quando os aplicativos a partir Office365 está instalado.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-225">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="4a3e9-226">Ele usa 6033 standard do RFC.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-226">It uses standard RFC 6033.</span></span> <span data-ttu-id="4a3e9-227">REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="4a3e9-227">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="4a3e9-228">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="4a3e9-228">installProgressDisplayLevel</span></span>|[<span data-ttu-id="4a3e9-229">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="4a3e9-229">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="4a3e9-230">Para especificar o nível de exibição para a interface de usuário de instalação de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-230">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="4a3e9-231">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-231">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="4a3e9-232">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="4a3e9-232">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="4a3e9-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a3e9-233">Boolean</span></span>|<span data-ttu-id="4a3e9-234">A propriedade para determinar se você desinstalar o MSI existente do Office se um pacote do app Office365 é implantado com o dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-234">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="4a3e9-235">targetVersion</span><span class="sxs-lookup"><span data-stu-id="4a3e9-235">targetVersion</span></span>|<span data-ttu-id="4a3e9-236">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-236">String</span></span>|<span data-ttu-id="4a3e9-237">A propriedade para representar a versão de destino específicos para o pacote do app Office365 que deve ser permaneceu implantada nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-237">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="4a3e9-238">updateVersion</span><span class="sxs-lookup"><span data-stu-id="4a3e9-238">updateVersion</span></span>|<span data-ttu-id="4a3e9-239">String</span><span class="sxs-lookup"><span data-stu-id="4a3e9-239">String</span></span>|<span data-ttu-id="4a3e9-240">A propriedade para representar a versão de atualização em que a versão de destino específico está disponível para o pacote de aplicativo Office365.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-240">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="4a3e9-241">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="4a3e9-241">officeConfigurationXml</span></span>|<span data-ttu-id="4a3e9-242">Binária</span><span class="sxs-lookup"><span data-stu-id="4a3e9-242">Binary</span></span>|<span data-ttu-id="4a3e9-243">A propriedade para representar o arquivo de configuração XML que pode ser especificado para o Office ProPlus Apps.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-243">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="4a3e9-244">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-244">Takes precedence over all other properties.</span></span> <span data-ttu-id="4a3e9-245">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-245">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="4a3e9-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a3e9-246">Response</span></span>
<span data-ttu-id="4a3e9-247">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-247">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a3e9-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a3e9-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a3e9-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a3e9-249">Request</span></span>
<span data-ttu-id="4a3e9-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1552

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="4a3e9-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a3e9-251">Response</span></span>
<span data-ttu-id="4a3e9-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a3e9-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1724

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```




