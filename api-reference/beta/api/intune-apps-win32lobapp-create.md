---
title: Criar win32LobApp
description: Crie um novo objeto de win32LobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: edd3e68d71cb2f31bb7b2f3fc0b24bde1e33768a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874367"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="221e0-103">Criar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="221e0-103">Create win32LobApp</span></span>

> <span data-ttu-id="221e0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="221e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="221e0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="221e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="221e0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="221e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="221e0-107">Crie um novo objeto de [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="221e0-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="221e0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="221e0-108">Prerequisites</span></span>
<span data-ttu-id="221e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="221e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="221e0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="221e0-111">Permission type</span></span>|<span data-ttu-id="221e0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="221e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="221e0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="221e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="221e0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="221e0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="221e0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="221e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="221e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="221e0-116">Not supported.</span></span>|
|<span data-ttu-id="221e0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="221e0-117">Application</span></span>|<span data-ttu-id="221e0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="221e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="221e0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="221e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="221e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="221e0-120">Request headers</span></span>
|<span data-ttu-id="221e0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="221e0-121">Header</span></span>|<span data-ttu-id="221e0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="221e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="221e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="221e0-123">Authorization</span></span>|<span data-ttu-id="221e0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="221e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="221e0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="221e0-125">Accept</span></span>|<span data-ttu-id="221e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="221e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="221e0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="221e0-127">Request body</span></span>
<span data-ttu-id="221e0-128">No corpo da solicitação, fornece uma representação JSON para o objeto win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="221e0-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="221e0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="221e0-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="221e0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="221e0-130">Property</span></span>|<span data-ttu-id="221e0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="221e0-131">Type</span></span>|<span data-ttu-id="221e0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="221e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="221e0-133">id</span><span class="sxs-lookup"><span data-stu-id="221e0-133">id</span></span>|<span data-ttu-id="221e0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-134">String</span></span>|<span data-ttu-id="221e0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="221e0-135">Key of the entity.</span></span> <span data-ttu-id="221e0-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="221e0-137">displayName</span></span>|<span data-ttu-id="221e0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-138">String</span></span>|<span data-ttu-id="221e0-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="221e0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="221e0-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-141">description</span><span class="sxs-lookup"><span data-stu-id="221e0-141">description</span></span>|<span data-ttu-id="221e0-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-142">String</span></span>|<span data-ttu-id="221e0-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-143">The description of the app.</span></span> <span data-ttu-id="221e0-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="221e0-145">publisher</span></span>|<span data-ttu-id="221e0-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-146">String</span></span>|<span data-ttu-id="221e0-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-147">The publisher of the app.</span></span> <span data-ttu-id="221e0-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="221e0-149">largeIcon</span></span>|[<span data-ttu-id="221e0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="221e0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="221e0-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="221e0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="221e0-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="221e0-153">createdDateTime</span></span>|<span data-ttu-id="221e0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="221e0-154">DateTimeOffset</span></span>|<span data-ttu-id="221e0-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-155">The date and time the app was created.</span></span> <span data-ttu-id="221e0-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="221e0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="221e0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="221e0-158">DateTimeOffset</span></span>|<span data-ttu-id="221e0-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="221e0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="221e0-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="221e0-161">isFeatured</span></span>|<span data-ttu-id="221e0-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="221e0-162">Boolean</span></span>|<span data-ttu-id="221e0-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="221e0-164">privacyInformationUrl</span></span>|<span data-ttu-id="221e0-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-165">String</span></span>|<span data-ttu-id="221e0-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="221e0-166">The privacy statement Url.</span></span> <span data-ttu-id="221e0-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="221e0-168">informationUrl</span></span>|<span data-ttu-id="221e0-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-169">String</span></span>|<span data-ttu-id="221e0-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="221e0-170">The more information Url.</span></span> <span data-ttu-id="221e0-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-172">owner</span><span class="sxs-lookup"><span data-stu-id="221e0-172">owner</span></span>|<span data-ttu-id="221e0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-173">String</span></span>|<span data-ttu-id="221e0-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="221e0-174">The owner of the app.</span></span> <span data-ttu-id="221e0-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-176">developer</span><span class="sxs-lookup"><span data-stu-id="221e0-176">developer</span></span>|<span data-ttu-id="221e0-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-177">String</span></span>|<span data-ttu-id="221e0-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-178">The developer of the app.</span></span> <span data-ttu-id="221e0-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-180">Observações</span><span class="sxs-lookup"><span data-stu-id="221e0-180">notes</span></span>|<span data-ttu-id="221e0-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-181">String</span></span>|<span data-ttu-id="221e0-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-182">Notes for the app.</span></span> <span data-ttu-id="221e0-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="221e0-184">uploadState</span></span>|<span data-ttu-id="221e0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="221e0-185">Int32</span></span>|<span data-ttu-id="221e0-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="221e0-186">The upload state.</span></span> <span data-ttu-id="221e0-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="221e0-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="221e0-188">publishingState</span></span>|[<span data-ttu-id="221e0-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="221e0-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="221e0-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-190">The publishing state for the app.</span></span> <span data-ttu-id="221e0-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="221e0-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="221e0-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="221e0-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="221e0-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="221e0-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="221e0-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="221e0-194">committedContentVersion</span></span>|<span data-ttu-id="221e0-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-195">String</span></span>|<span data-ttu-id="221e0-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="221e0-196">The internal committed content version.</span></span> <span data-ttu-id="221e0-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="221e0-198">fileName</span><span class="sxs-lookup"><span data-stu-id="221e0-198">fileName</span></span>|<span data-ttu-id="221e0-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-199">String</span></span>|<span data-ttu-id="221e0-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="221e0-200">The name of the main Lob application file.</span></span> <span data-ttu-id="221e0-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="221e0-202">size</span><span class="sxs-lookup"><span data-stu-id="221e0-202">size</span></span>|<span data-ttu-id="221e0-203">Int64</span><span class="sxs-lookup"><span data-stu-id="221e0-203">Int64</span></span>|<span data-ttu-id="221e0-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="221e0-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="221e0-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="221e0-206">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="221e0-206">installCommandLine</span></span>|<span data-ttu-id="221e0-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-207">String</span></span>|<span data-ttu-id="221e0-208">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="221e0-208">The command line to install this app</span></span>|
|<span data-ttu-id="221e0-209">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="221e0-209">uninstallCommandLine</span></span>|<span data-ttu-id="221e0-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-210">String</span></span>|<span data-ttu-id="221e0-211">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="221e0-211">The command line to uninstall this app</span></span>|
|<span data-ttu-id="221e0-212">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="221e0-212">applicableArchitectures</span></span>|[<span data-ttu-id="221e0-213">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="221e0-213">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="221e0-214">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="221e0-214">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="221e0-215">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="221e0-215">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="221e0-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="221e0-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="221e0-217">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="221e0-217">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="221e0-218">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="221e0-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="221e0-219">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="221e0-219">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="221e0-220">Int32</span><span class="sxs-lookup"><span data-stu-id="221e0-220">Int32</span></span>|<span data-ttu-id="221e0-221">O valor para o espaço livre em disco mínimo que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-221">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="221e0-222">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="221e0-222">minimumMemoryInMB</span></span>|<span data-ttu-id="221e0-223">Int32</span><span class="sxs-lookup"><span data-stu-id="221e0-223">Int32</span></span>|<span data-ttu-id="221e0-224">O valor para o mínimo de memória físico que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-224">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="221e0-225">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="221e0-225">minimumNumberOfProcessors</span></span>|<span data-ttu-id="221e0-226">Int32</span><span class="sxs-lookup"><span data-stu-id="221e0-226">Int32</span></span>|<span data-ttu-id="221e0-227">O valor para o número mínimo de processadores, que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-227">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="221e0-228">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="221e0-228">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="221e0-229">Int32</span><span class="sxs-lookup"><span data-stu-id="221e0-229">Int32</span></span>|<span data-ttu-id="221e0-230">O valor para a velocidade de CPU mínima, que é necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-230">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="221e0-231">detectionRules</span><span class="sxs-lookup"><span data-stu-id="221e0-231">detectionRules</span></span>|<span data-ttu-id="221e0-232">coleção [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="221e0-233">As regras de detecção para detectar app Win32 linha de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="221e0-233">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="221e0-234">installExperience</span><span class="sxs-lookup"><span data-stu-id="221e0-234">installExperience</span></span>|[<span data-ttu-id="221e0-235">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="221e0-235">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="221e0-236">A experiência da instalação para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="221e0-236">The install experience for this app.</span></span>|
|<span data-ttu-id="221e0-237">returnCodes</span><span class="sxs-lookup"><span data-stu-id="221e0-237">returnCodes</span></span>|<span data-ttu-id="221e0-238">coleção [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="221e0-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="221e0-239">Os códigos de retorno para lançar o comportamento da instalação.</span><span class="sxs-lookup"><span data-stu-id="221e0-239">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="221e0-240">msiInformation</span><span class="sxs-lookup"><span data-stu-id="221e0-240">msiInformation</span></span>|[<span data-ttu-id="221e0-241">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="221e0-241">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="221e0-242">Os detalhes do MSI se este aplicativo Win32 é um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="221e0-242">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="221e0-243">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="221e0-243">setupFilePath</span></span>|<span data-ttu-id="221e0-244">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="221e0-244">String</span></span>|<span data-ttu-id="221e0-245">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="221e0-245">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="221e0-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="221e0-246">Response</span></span>
<span data-ttu-id="221e0-247">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [win32LobApp](../resources/intune-apps-win32lobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="221e0-247">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="221e0-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="221e0-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="221e0-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="221e0-249">Request</span></span>
<span data-ttu-id="221e0-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="221e0-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2264

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="221e0-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="221e0-251">Response</span></span>
<span data-ttu-id="221e0-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="221e0-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2372

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```





