task default: [:'thrift:gen-rb']

task :'thrift:gen-rb' do
  sh('mkdir -p lib/thrift')
  sh("for i in $(find #{ENV['DIR'] || '.'} -name '*.thrift'); do thrift -out lib/thrift --gen rb $i; done")
end
