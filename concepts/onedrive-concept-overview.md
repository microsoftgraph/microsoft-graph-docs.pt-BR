---
title: Visão geral da API de armazenamento de arquivos do OneDrive
description: O OneDrive é a central de arquivos no Microsoft 365.
ms.localizationpriority: high
ms.prod: onedrive
ms.custom: scenarios:getting-started
ms.openlocfilehash: 080d05a3fbba08108b14048968dee47fa1cd2dbc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019080"
---
# <a name="onedrive-file-storage-api-overview"></a>Visão geral da API de armazenamento de arquivos do OneDrive

O OneDrive é a central de arquivos no Microsoft 365.
As pessoas trabalham com arquivos em vários contextos, como o Microsoft Teams, grupos, SharePoint e muito mais.
Com o OneDrive, os usuários podem acessar esses arquivos independentemente de onde eles estejam armazenados; com o Microsoft Graph, você pode usar uma única API para trabalhar com eles.

Os arquivos no Microsoft 365 são armazenados em [unidades][Drive API].
Os usuários podem armazenar arquivos em uma unidade pessoal, o OneDrive pessoal, ou em uma unidade compartilhada com a tecnologia de uma biblioteca de documentos do [SharePoint][].
A flexibilidade do OneDrive permite que os usuários colaborem como acharem melhor para eles.
Os usuários podem compartilhar links para arquivos, copiar ou mover arquivos para unidades da equipe ou até mesmo anexar arquivos do OneDrive às mensagens de email no Outlook.

> [!VIDEO https://www.youtube-nocookie.com/embed/vG-hQxFHCAE]

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a>Por que se integrar ao armazenamento de arquivos do OneDrive na nuvem?

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a>Utilize um ecossistema com bilhões de arquivos

Os usuários do OneDrive podem acessar seus arquivos de qualquer dispositivo, online ou offline, e compartilhar arquivos com pessoas de dentro ou de fora da organização.
O OneDrive permite a coautoria em tempo real em aplicativos conhecidos, como o Word, o Excel e o PowerPoint.
Os arquivos ficam ainda melhores com miniaturas avançadas para centenas de formatos, transmissão de vídeo, análises, entre outros, com base na tecnologia do Microsoft Graph.
Os dados no OneDrive são protegidos com recursos avançados de segurança, conformidade e a criptografia em que os clientes confiam.

Com mais de 500 milhões de dispositivos executando o aplicativo do OneDrive e mais de 85% das empresas da Fortune 500 usando o OneDrive for Business, ao integrar o aplicativo ao OneDrive você pode se conectar com milhões de clientes, alunos e usuários corporativos e interagir com os clientes de onde eles já trabalham todo dia.

### <a name="store-your-apps-files-in-a-powerful-cloud"></a>Armazenar os arquivos do seu aplicativo em uma nuvem avançada

Quando você armazena seus arquivos no OneDrive, seu aplicativo pode utilizar os recursos da nuvem da Microsoft e seus usuários podem acessar os arquivos de qualquer lugar.
Use a SDK do [seletor de arquivos][] para rapidamente abrir, baixar, salvar ou compartilhar os arquivos armazenados no OneDrive do próprio aplicativo, usando a mesma experiência que os usuários do OneDrive já conhecem.
Obtenha informações sobre os arquivos selecionados diretamente do SDK do seletor ou use diretamente as APIs do Microsoft Graph para interagir de forma mais profunda com os arquivos.
Use [pastas especiais][] para armazenar arquivos em locais conhecidos no OneDrive, como `Documents` e `Camera Roll`, ou crie uma pasta pessoal para o seu aplicativo.

### <a name="bring-your-app-straight-to-users-within-onedrive"></a>Disponibilizar o seu aplicativo diretamente para os usuários no OneDrive

Os clientes do OneDrive podem usar ou iniciar o seu aplicativo diretamente do OneDrive para abrir, editar ou visualizar arquivos.
Use as extensões do [manipulador de arquivos][] do OneDrive para fornecer ícones e visualizações para as suas próprias extensões de arquivo personalizado, adicionar o seu aplicativo ao botão **Novo** ou até mesmo adicionar as suas próprias ações personalizadas à barra de menus para iniciar o aplicativo.

### <a name="work-with-content-in-formats-your-app-understands"></a>Trabalhar com conteúdo em formatos que o seu aplicativo entende

O aplicativo pode obter o conteúdo do arquivo no formato que for mais conveniente para você.
O aplicativo pode exibir [miniaturas][] de tamanho personalizado para centenas de formatos diferentes de arquivo.
Você pode baixar arquivos em vários [formatos][] alternativos, como PDF.
Você pode inclusive inserir visualizadores de arquivo do OneDrive no seu aplicativo usando a API de [visualização][] (beta).

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a>Trabalhar com conteúdo e metadados de arquivo sem baixar o binário

Com o Microsoft Graph, é possível acessar conteúdo avançado por meio de APIs REST sem precisar baixar o binário.
Explore os metadados extraídos dos arquivos de [foto][], [áudio][] e [vídeo][].
Use a [API do Excel][] para trabalhar diretamente com os dados brutos armazenados em uma pasta de trabalho do Excel.
Use a [API de anotações][] para acessar o conteúdo dos blocos de anotações do OneNote.

### <a name="react-to-file-changes"></a>Reagir a alterações de arquivo

Com o [webhooks][], seu aplicativo pode ser notificado sobre a alteração de arquivos, o que possibilita que você reaja rapidamente.
Use a [API delta][] para ver o que foi alterado desde a última vez em que o aplicativo foi sincronizado com a nuvem.

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API deste serviço?

- [API de armazenamento de arquivos do OneDrive no Microsoft Graph versão 1.0](/graph/api/resources/onedrive?view=graph-rest-1.0)
- [API de armazenamento de arquivos do OneDrive no Microsoft Graph beta](/graph/api/resources/onedrive?view=graph-rest-beta)

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre [como usar a API do OneDrive][Drive API] no Microsoft Graph v1.0.

[SharePoint]: sharepoint-concept-overview.md
[seletor de arquivos]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[manipulador de arquivos]: /onedrive/developer/file-handlers
[pastas especiais]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[API de anotações]: integrate-with-onenote.md
[API do Excel]: /graph/api/resources/excel?view=graph-rest-1.0
[REST API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[API delta]: /graph/api/driveitem-delta?view=graph-rest-1.0
[vídeo]: /graph/api/resources/video?view=graph-rest-1.0
[foto]: /graph/api/resources/photo?view=graph-rest-1.0
[áudio]: /graph/api/resources/audio?view=graph-rest-1.0
[formatos]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[miniaturas]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[visualização]: /graph/api/driveitem-preview?view=graph-rest-beta
[webhooks]: /graph/api/resources/webhooks?view=graph-rest-1.0
[Drive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
