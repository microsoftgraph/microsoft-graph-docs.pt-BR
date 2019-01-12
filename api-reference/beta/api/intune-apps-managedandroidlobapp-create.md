---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 56e8a68a817bbca8e575d34f69d55f5bd3dccba5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930030"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="1c796-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="1c796-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="1c796-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1c796-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c796-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1c796-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c796-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1c796-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c796-107">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c796-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c796-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c796-108">Prerequisites</span></span>
<span data-ttu-id="1c796-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c796-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c796-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c796-111">Permission type</span></span>|<span data-ttu-id="1c796-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c796-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c796-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c796-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c796-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c796-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c796-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c796-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c796-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c796-116">Not supported.</span></span>|
|<span data-ttu-id="1c796-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c796-117">Application</span></span>|<span data-ttu-id="1c796-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c796-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c796-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c796-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1c796-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c796-120">Request headers</span></span>
|<span data-ttu-id="1c796-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c796-121">Header</span></span>|<span data-ttu-id="1c796-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c796-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c796-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c796-123">Authorization</span></span>|<span data-ttu-id="1c796-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c796-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c796-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c796-125">Accept</span></span>|<span data-ttu-id="1c796-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c796-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c796-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c796-127">Request body</span></span>
<span data-ttu-id="1c796-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="1c796-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="1c796-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="1c796-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="1c796-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c796-130">Property</span></span>|<span data-ttu-id="1c796-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c796-131">Type</span></span>|<span data-ttu-id="1c796-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c796-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c796-133">id</span><span class="sxs-lookup"><span data-stu-id="1c796-133">id</span></span>|<span data-ttu-id="1c796-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-134">String</span></span>|<span data-ttu-id="1c796-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1c796-135">Key of the entity.</span></span> <span data-ttu-id="1c796-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1c796-137">displayName</span></span>|<span data-ttu-id="1c796-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-138">String</span></span>|<span data-ttu-id="1c796-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1c796-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1c796-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-141">description</span><span class="sxs-lookup"><span data-stu-id="1c796-141">description</span></span>|<span data-ttu-id="1c796-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-142">String</span></span>|<span data-ttu-id="1c796-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-143">The description of the app.</span></span> <span data-ttu-id="1c796-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1c796-145">publisher</span></span>|<span data-ttu-id="1c796-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-146">String</span></span>|<span data-ttu-id="1c796-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-147">The publisher of the app.</span></span> <span data-ttu-id="1c796-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1c796-149">largeIcon</span></span>|[<span data-ttu-id="1c796-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1c796-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1c796-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1c796-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1c796-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c796-153">createdDateTime</span></span>|<span data-ttu-id="1c796-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c796-154">DateTimeOffset</span></span>|<span data-ttu-id="1c796-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-155">The date and time the app was created.</span></span> <span data-ttu-id="1c796-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c796-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1c796-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c796-158">DateTimeOffset</span></span>|<span data-ttu-id="1c796-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1c796-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1c796-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1c796-161">isFeatured</span></span>|<span data-ttu-id="1c796-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c796-162">Boolean</span></span>|<span data-ttu-id="1c796-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1c796-164">privacyInformationUrl</span></span>|<span data-ttu-id="1c796-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-165">String</span></span>|<span data-ttu-id="1c796-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1c796-166">The privacy statement Url.</span></span> <span data-ttu-id="1c796-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1c796-168">informationUrl</span></span>|<span data-ttu-id="1c796-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-169">String</span></span>|<span data-ttu-id="1c796-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1c796-170">The more information Url.</span></span> <span data-ttu-id="1c796-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-172">owner</span><span class="sxs-lookup"><span data-stu-id="1c796-172">owner</span></span>|<span data-ttu-id="1c796-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-173">String</span></span>|<span data-ttu-id="1c796-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1c796-174">The owner of the app.</span></span> <span data-ttu-id="1c796-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-176">developer</span><span class="sxs-lookup"><span data-stu-id="1c796-176">developer</span></span>|<span data-ttu-id="1c796-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-177">String</span></span>|<span data-ttu-id="1c796-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-178">The developer of the app.</span></span> <span data-ttu-id="1c796-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-180">Observações</span><span class="sxs-lookup"><span data-stu-id="1c796-180">notes</span></span>|<span data-ttu-id="1c796-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-181">String</span></span>|<span data-ttu-id="1c796-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-182">Notes for the app.</span></span> <span data-ttu-id="1c796-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1c796-184">uploadState</span></span>|<span data-ttu-id="1c796-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1c796-185">Int32</span></span>|<span data-ttu-id="1c796-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1c796-186">The upload state.</span></span> <span data-ttu-id="1c796-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1c796-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1c796-188">publishingState</span></span>|[<span data-ttu-id="1c796-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1c796-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1c796-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-190">The publishing state for the app.</span></span> <span data-ttu-id="1c796-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1c796-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1c796-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c796-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1c796-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1c796-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1c796-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="1c796-194">appAvailability</span></span>|[<span data-ttu-id="1c796-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="1c796-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="1c796-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-196">The Application's availability.</span></span> <span data-ttu-id="1c796-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1c796-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="1c796-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="1c796-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="1c796-199">version</span><span class="sxs-lookup"><span data-stu-id="1c796-199">version</span></span>|<span data-ttu-id="1c796-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-200">String</span></span>|<span data-ttu-id="1c796-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c796-201">The Application's version.</span></span> <span data-ttu-id="1c796-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="1c796-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1c796-203">committedContentVersion</span></span>|<span data-ttu-id="1c796-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-204">String</span></span>|<span data-ttu-id="1c796-205">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="1c796-205">The internal committed content version.</span></span> <span data-ttu-id="1c796-206">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1c796-207">fileName</span><span class="sxs-lookup"><span data-stu-id="1c796-207">fileName</span></span>|<span data-ttu-id="1c796-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-208">String</span></span>|<span data-ttu-id="1c796-209">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="1c796-209">The name of the main Lob application file.</span></span> <span data-ttu-id="1c796-210">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1c796-211">size</span><span class="sxs-lookup"><span data-stu-id="1c796-211">size</span></span>|<span data-ttu-id="1c796-212">Int64</span><span class="sxs-lookup"><span data-stu-id="1c796-212">Int64</span></span>|<span data-ttu-id="1c796-213">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="1c796-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="1c796-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1c796-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1c796-215">packageId</span><span class="sxs-lookup"><span data-stu-id="1c796-215">packageId</span></span>|<span data-ttu-id="1c796-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-216">String</span></span>|<span data-ttu-id="1c796-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="1c796-217">The package identifier.</span></span>|
|<span data-ttu-id="1c796-218">identityName</span><span class="sxs-lookup"><span data-stu-id="1c796-218">identityName</span></span>|<span data-ttu-id="1c796-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-219">String</span></span>|<span data-ttu-id="1c796-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1c796-220">The Identity Name.</span></span>|
|<span data-ttu-id="1c796-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1c796-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1c796-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1c796-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="1c796-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1c796-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1c796-224">versionName</span><span class="sxs-lookup"><span data-stu-id="1c796-224">versionName</span></span>|<span data-ttu-id="1c796-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-225">String</span></span>|<span data-ttu-id="1c796-226">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="1c796-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1c796-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="1c796-227">versionCode</span></span>|<span data-ttu-id="1c796-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-228">String</span></span>|<span data-ttu-id="1c796-229">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="1c796-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1c796-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1c796-230">identityVersion</span></span>|<span data-ttu-id="1c796-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c796-231">String</span></span>|<span data-ttu-id="1c796-232">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="1c796-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1c796-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c796-233">Response</span></span>
<span data-ttu-id="1c796-234">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c796-234">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c796-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c796-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c796-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c796-236">Request</span></span>
<span data-ttu-id="1c796-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c796-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1443

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="1c796-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c796-238">Response</span></span>
<span data-ttu-id="1c796-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c796-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1551

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





